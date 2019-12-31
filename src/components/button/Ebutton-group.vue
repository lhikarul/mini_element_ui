<template>
  <div class="e-button-group">
    <slot></slot>
  </div>
</template>
<script>
  export default {
    name: 'ElButtonGroup'
  };
</script>

<style lang="scss" scoped>
.e-button-group {
    display: inline-block;
    vertical-align: middle;

    .e-button {
        float: left;
        position: relative;

        &--primary:last-child {
            border-left-color: hsla(0,0%,100%,.5);
        }

        &:first-child {
            border-top-right-radius: 0;
            border-bottom-right-radius: 0;
        }

        &:not(:last-child) {
            margin-right: -1px;
        }
    }

    .e-button + .e-button {
        margin-left: 0;
    }
}
</style>