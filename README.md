# vue-element-ui 2.13.0 源碼分析

## 介紹
深入分析 element ui 源碼，並實作一個 mini-element-ui

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### button 



``` 
    <el-row>
      <e-button>默认按钮</e-button>
      <e-button type="primary">主要按钮</e-button>
      <e-button type="success">成功按钮</e-button>
      <e-button type="info">信息按钮</e-button>
      <e-button type="warning">警告按钮</e-button>
      <e-button type="danger">危险按钮</e-button>
    </el-row>

    <el-row>
      <e-button plain>朴素按钮</e-button>
      <e-button type="primary" plain>主要按钮</e-button>
      <e-button type="success" plain>成功按钮</e-button>
      <e-button type="info" plain>信息按钮</e-button>
      <e-button type="warning" plain>警告按钮</e-button>
      <e-button type="danger" plain>危险按钮</e-button>
    </el-row>

    <el-row>
      <e-button round>圆角按钮</e-button>
      <e-button type="primary" round>主要按钮</e-button>
      <e-button type="success" round>成功按钮</e-button>
      <e-button type="info" round>信息按钮</e-button>
      <e-button type="warning" round>警告按钮</e-button>
      <e-button type="danger" round>危险按钮</e-button>
    </el-row>

    <el-row>
      <e-button circle></e-button>
      <e-button type="primary" circle></e-button>
      <e-button type="success" circle></e-button>
      <e-button type="info"  circle></e-button>
      <e-button type="warning" circle></e-button>
      <e-button type="danger" circle></e-button>
    </el-row>
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
