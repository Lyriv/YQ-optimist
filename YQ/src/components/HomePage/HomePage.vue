<template>
  <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="工作中的知识" name="first">用户管理</el-tab-pane>
    <el-tab-pane label="自己拓展的知识" name="second">配置管理</el-tab-pane>
    <el-tab-pane label="小小项目" name="third">角色管理</el-tab-pane>
  </el-tabs>
</template>
<script>
  export default {
    data() {
      return {
        activeName: 'first'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    }
  };
</script>