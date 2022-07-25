<!-- list父组件 -->
<template>
  <div>
    <list-item :str="str" :obj="obj" :arr="arr"></list-item>
    <div>
        <span v-bind:title="message">
        鼠标悬停几秒钟查看此处动态绑定的提示信息！
        </span>
    </div>

  </div>
</template>

<script lang="ts">
import ListItem from '../components/ListItem.vue'
export default {
  data() {
    return {
      str: "给子组件传值",
      obj: { msg: "给子组件传值" },
      arr: [1,2,3],
      message:'页面加载于'+ new Date().toLocaleString()
    };
  },
  components:{
    ListItem    
  }
};
</script>

<style>
</style>