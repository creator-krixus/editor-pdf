<script setup>
import HelloWorld from './components/HelloWorld.vue'
import WebViewer from "./components/WebViewer.vue"
</script>

<template>
  <HelloWorld />
  <WebViewer
    initialDoc="https://pdftron.s3.amazonaws.com/downloads/pl/webviewer-demo.pdf" />
</template>

<style>
</style>
