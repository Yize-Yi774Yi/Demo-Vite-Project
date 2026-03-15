<template>{{ message }}</template>
<script setup>
import { ref } from 'vue'
const message = ref('四川欢迎你ref！')
setTimeout(() => {
    message.value = '成都欢迎你！'
}, 5000)
</script>