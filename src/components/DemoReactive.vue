<template>{{ obj.message }}</template>
<script setup>
import { reactive } from 'vue'
const obj = reactive({ message: '四川欢迎你！reactive' })
setTimeout(() => {
    obj.message = '成都欢迎你！'
}, 5000)
</script>