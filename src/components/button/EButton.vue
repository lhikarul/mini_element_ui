<template>
    <button type="button" class="mt-30 e-button" :class="['e-button--' + type,{
        'is-plain': plain,
        'is-round': round,
        'is-circle': circle
    }]">
        <span>
            <slot></slot>
        </span>
    </button>
</template>

<script>
    export default {
        name: 'EButton',
        props: {
            type: {
                type: String,
                default: 'default'
            },
            plain: Boolean,
            round: Boolean,
            circle: Boolean
        }
    }
</script>

<style lang="scss" scoped>
.mt-30 {
    margin-top: 30px !important; 
}
.e-button {
    display: inline-block;
    line-height: 1;
    white-space: nowrap;
    cursor: pointer;
    background: #fff;
    border: 1px solid #dcdfe6;
    color: #606266;
    -webkit-appearance: none;
    text-align: center;
    box-sizing: border-box;
    outline: none;
    margin: 0;
    transition: .1s;
    font-weight: 500;
    -moz-user-select: none;
    -webkit-user-select: none;
    -ms-user-select: none;
    padding: 12px 20px;
    font-size: 14px;
    border-radius: 4px;

    & + & {
        margin-left: 10px;
    }

    &:focus, &:hover {
        color: #409eff;
        border-color: #c6e2ff;
        background-color: #ecf5ff
    }

    &:active {
        color: #3a8ee6;
        border-color: #3a8ee6;
        outline: none
    }

    &.is-plain {
        &:focus, &:hover {
            background: #fff;
            border-color: #409eff;
            color: #409eff;
        }

        &:active {
            background: #fff;
            outline: none;
        }
    }

    &.is-round {
        border-radius: 20px;
        padding: 12px 23px;
    }

    &.is-circle {
        border-radius: 50%;
        padding: 12px;
    }

    &--primary {
        color: #fff;
        background-color: #409eff;
        border-color: #409eff;

        &:hover, &:focus {
            background: #66b1ff;
            border-color: #66b1ff;
            color: #fff;
        }

        &:active {
            outline: none;
        }

        &.is-plain {
            color: #409eff;
            background: #ecf5ff;
            border-color: #b3d8ff;
        }

        &.is-plain:focus, &.is-plain:hover {
            background: #409eff;
            border-color: #409eff;
            color: #fff;
        }

        &.is-plain:active {
            background: #3a8ee6;
            border-color: #3a8ee6;
            color: #fff;
            outline: none;
        }

    }

    &--success {
        color: #fff;
        background-color: #67c23a;
        border-color: #67c23a;

        &:focus, &:hover {
            background: #85ce61;
            border-color: #85ce61;
            color: #fff;
        }

        &:active {
            outline: none;
        }

        &.is-active, &:active {
            background: #5daf34;
            border-color: #5daf34;
            color: #fff;
        }

        &.is-plain {
            color: #67c23a;
            background: #f0f9eb;
            border-color: #c2e7b0;
        }

        &.is-plain:focus, &.is-plain:hover {
            background: #67c23a;
            border-color: #67c23a;
            color: #fff;
        }

        &.is-plain:active {
            background: #5daf34;
            border-color: #5daf34;
            color: #fff;
            outline: none;
        }
    }

    &--warning {
        color: #fff;
        background-color: #e6a23c;
        border-color: #e6a23c;

        &:focus, &:hover {
            background: #ebb563;
            border-color: #ebb563;
            color: #fff;
        }

        &:active {
            outline: none;
        }

        &.is-active, &:active {
            background: #cf9236;
            border-color: #cf9236;
            color: #fff;
        }

         &.is-plain {
            color: #e6a23c;
            background: #fdf6ec;
            border-color: #f5dab1;
        }

        &.is-plain:focus, &.is-plain:hover {
            background: #e6a23c;
            border-color: #e6a23c;
            color: #fff;
        }

        &.is-plain:active {
            background: #cf9236;
            border-color: #cf9236;
            color: #fff;
            outline: none;
        }
    }

    &--danger {
        color: #fff;
        background-color: #f56c6c;
        border-color: #f56c6c;

         &:focus, &:hover {
            background: #f78989;
            border-color: #f78989;
            color: #fff;
        }

        &:active {
            outline: none;
        }

        &.is-active, &:active {
            background: #dd6161;
            border-color: #dd6161;
            color: #fff;
        }

        &.is-plain {
            color: #f56c6c;
            background: #fef0f0;
            border-color: #fbc4c4;
        }

        &.is-plain:focus, &.is-plain:hover {
            background: #f56c6c;
            border-color: #f56c6c;
            color: #fff;
        }

        &.is-plain:active {
            background: #dd6161;
            border-color: #dd6161;
            color: #fff;
            outline: none;
        }
    }

    &--info {
        color: #fff;
        background-color: #909399;
        border-color: #909399;

         &:focus, &:hover {
            background: #a6a9ad;
            border-color: #a6a9ad;
            color: #fff;
        }

        &:active {
            outline: none;
        }

        &.is-active, &:active {
            background: #82848a;
            border-color: #82848a;
            color: #fff;
        }

        &.is-plain {
            color: #909399;
            background: #f4f4f5;
            border-color: #d3d4d6;
        }

        &.is-plain:focus, &.is-plain:hover {
            background: #909399;
            border-color: #909399;
            color: #fff;
        }

        &.is-plain:active {
            background: #82848a;
            border-color: #82848a;
            color: #fff;
            outline: none;
        }
    }
}
</style>