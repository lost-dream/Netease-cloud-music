<template>
  <div class="logo-box">
    <img class="logo vite" src="./assets/vite.svg" />
    <img class="logo electron" src="./assets/electron.svg" />
    <img class="logo vue" src="./assets/vue.svg" />
  </div>
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
  <div class="static-public">
    Place static files into the <code>/public</code> folder
    <img style="width: 77px" :src="'./node.png'" />
  </div>
</template>

<script setup lang="ts">
  import HelloWorld from './components/HelloWorld.vue';
</script>

<style>
  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .logo-box {
    display: flex;
    width: 100%;
    justify-content: center;
  }

  .static-public {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .static-public code {
    background-color: #eee;
    padding: 2px 4px;
    margin: 0 4px;
    border-radius: 4px;
    color: #304455;
  }

  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: 0.75s;
  }

  .logo.vite:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }

  .logo.electron:hover {
    filter: drop-shadow(0 0 2em #9feaf9);
  }

  .logo.vue:hover {
    filter: drop-shadow(0 0 2em #42b883aa);
  }
</style>
