<template>
  <div class="home">
    <p id="aa"></p>
  </div>
</template>
<script setup lang="ts">
import TypeIt from "typeit";
import {onMounted} from "vue";

const init = () => {
  new TypeIt("#aa", { strings: "你好！欢迎来到我的站点。", speed: 200 }).go();
}

onMounted(() => {
  init();
})

</script>
<style scoped>
#aa {
  font-size: 60px;
  font-weight: bold;
  font-family: serif;
  background: linear-gradient(to right, #39ff00, #ff0000);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  height: calc(100vh - 0px);
  background-image: url("/pexels-yating-yang-426041335-20445455.jpg");
  background-repeat: no-repeat;
  background-size:100% 100%;
  background-attachment:fixed;
}
</style>
