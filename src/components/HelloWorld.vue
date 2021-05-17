<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      {{ $t('app.linktoDocument') }}
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">{{ $t('app.title') }}</a>
  </p>

  <p>主题</p>

  <button @click="state.count++">count is: {{ state.count }}</button>
  <p><code>components/HelloWorld.vue</code> to test hot module replacement.</p>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String,
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
