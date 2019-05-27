# vue-picviewer
> A Vue component to picture view


<p>
  <a href="https://npmcharts.com/compare/vue-picviewer?minimal=true"><img src="https://img.shields.io/npm/dm/vue-picviewer.svg" alt="Downloads"></a>
  <a href="https://www.npmjs.com/package/vue-picviewer"><img src="https://img.shields.io/npm/v/vue-picviewer.svg" alt="Version"></a>
  <a href="https://www.npmjs.com/package/vue-picviewer"><img src="https://img.shields.io/npm/l/vue-picviewer.svg" alt="License"></a>
</p>

### Install
通过```npm install vue-picviewer -save``` 安装到相应的项目下或者```yarn add vue-picviewer```

### How to use
```vue
import Picview from 'vue-picviewer';
import Css from 'vue-picviewer/dist/vue-picviewer.min.css'
export default {
  name: 'app',
  components:{
     Picview
  },
}
```
### Demo

```vue
<template>
  <div id="app">
    <div class="a">
      <Picview :imgdata="imgdata1" width="100px;" />
    </div>
    <div class="a">
      <Picview :imgdata="imgdata2" :props="{thumbnail:'src',original:'src'}" width="200px;" />
    </div>
  </div>
</template>
import Picview from "vue-picviewer";
import Css from "vue-picviewer/dist/vue-picviewer.min.css";
export default {
    name: "App",
    components: {
        Picview
    },
    data() {
        return {
            imgdata1: [
                "https://www.gravatar.com/avatar/40206d98ff6e85da457c341e4a4ea437",
                "https://www.gravatar.com/avatar/40206d98ff6e85da457c341e4a4ea437"
            ],
            imgdata2: [
                {
                    src:
                        "https://www.gravatar.com/avatar/40206d98ff6e85da457c341e4a4ea437"
                },
                {
                    src:
                        "https://www.gravatar.com/avatar/40206d98ff6e85da457c341e4a4ea437"
                }
            ]
        };
    }
};
</script>

<style>
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
```
### Attributes

| 属性        |类型         |   参数                                   |  说明    |
| ----------- |------------| ---------------------------------------- |----------|
|imgdata|Array,Object| Array:['http://src','http://src'];Object ||
|props|Object|"thumbnail":缩略图的数据对象属性，"original":原图的数据对象属性 |仅imgdata属性为Object可用|
|width|String||缩略图的宽度|
|height|String||缩略图的高度|
### Example
![img](https://github.com/chenyeah/vue-picviewer/raw/master/docs/demo.gif)
