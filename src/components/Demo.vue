<template>{{ message }}</template>

<script setup>
let message = '四川欢迎你demo！'
setTimeout(() => {
    console.log('跟新前数据message;' + message)
    message = '成都欢迎你！'
    console.log('跟新后数据message;' + message)
}, 5000)
</script>