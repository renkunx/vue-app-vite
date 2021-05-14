<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite11211111111111111111111111" />
  <p>{{ $t('hello') }}</p>
  <p>{{ $t('translate') }}</p>
  <title :name="$t('component.title')">2222222</title>
  <select name="language" id="" @change="handleLanguageChange">
    <option value="zh">中文</option>
    <option value="en">英文</option>
  </select>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  components: {
    HelloWorld,
  },
  props: {},
  methods: {
    handleLanguageChange: function (e) {
      this.$i18n.locale = e.target.value
    },
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
title {
  display: block;
}
</style>
