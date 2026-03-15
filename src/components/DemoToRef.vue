<template>
    <div>message的值：{{ message }}</div>
    <div>obj.message的值：{{ obj.message }}</div>
</template>
<script setup>
import { reactive, toRef } from 'vue'
const obj = reactive({ message: '四川欢迎你！' })
const message = toRef(obj, 'message')
setTimeout(() => {
    message.value = '成都欢迎你！'
}, 5000)
</script>