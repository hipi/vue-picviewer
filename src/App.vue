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

<script>
import Picview from "./Picview.vue";

export default {
    name: "app",
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
}
body {
    margin: 0;
    padding: 0;
}
.a {
    margin-bottom: 40px;
}
</style>
