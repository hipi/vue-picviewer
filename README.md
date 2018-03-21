# vue-picview
> A Vue component to picture view

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
# 使用组件
通过```npm install vue-picview -save``` 安装到相应的项目下或者```yarn add vue-picview```

### 项目中引入
```vue
import Picview from 'vue-marquee-ho';
import Css from 'vue-marquee-ho/dist/vue-marquee.min.css'
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
import Picview from "vue-picview";
import Css from "vue-picview/dist/vue-picview.min.css";
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
### 效果
