<template>
    <div>
        <div>{{str}}</div>
        <div>{{obj}}</div>
        <div>{{arr}}</div>
    </div>
</template>

<script lang="ts">
    export default {
        props: {
            str: String, // Props是字符串
            obj: Object,  // props是对象
            arr: Array    // props是数组
        }
    }
</script>

<style lang="less" scoped>

</style>