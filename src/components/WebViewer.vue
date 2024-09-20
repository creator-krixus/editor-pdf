<script setup>
import { ref, onMounted } from "vue"
import WebViewer from "@pdftron/webviewer"
const props = defineProps({
    initialDoc: String,
})
const viewerDiv = ref(null)
onMounted(() => {
    const path = `${import.meta.env.BASE_URL}lib`
    WebViewer({ path, initialDoc: props.initialDoc }, viewerDiv.value)
})
</script>
<template>
    <div id="webViewer" ref="viewerDiv">

    </div>
</template>
<style>
#webViewer {
    width: 1280px;
    height: 200vh;
}
</style>