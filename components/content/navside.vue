<template>
    <div>     
        <el-menu :default-active="activeIndex" class="el-menu-demo" style="height: 70px" mode="horizontal" @select="handleSelect"
        background-color="#0D78E7" text-color="#fff" active-text-color="#fff">
        <el-menu-item style="margin-left: 150px;" index="1">Processing Center</el-menu-item>
        <el-submenu index="2">
            <template slot="title">Workspace</template>
            <el-menu-item index="2-1">item one</el-menu-item>
            <el-menu-item index="2-2">item two</el-menu-item>
            <el-menu-item index="2-3">item three</el-menu-item>
            <el-submenu index="2-4">
            <template slot="title">item four</template>
            <el-menu-item index="2-4-1">item one</el-menu-item>
            <el-menu-item index="2-4-2">item two</el-menu-item>
            <el-menu-item index="2-4-3">item three</el-menu-item>
            </el-submenu>
        </el-submenu>
        <el-menu-item index="3" disabled>Info</el-menu-item>
        <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">Orders</a></el-menu-item>
        <el-menu-item style="float: right;
        margin-right: 150px">Logout</el-menu-item>
        
        <input
        style="margin-top: 15px;
        height: 30px;
        width: 350px;
        border-radius: 4px;
        display: inline-block;
        border: none;
        box-sizing: border-box;
        float: right;
        margin-right: 30px;
        " type="text">
        <el-menu-item
        style="float: right;"
        >Search</el-menu-item>
        </el-menu>
    </div>
</template>
<script>
  export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      },
    },
  }
</script>

<style scoped>
    a{
        text-decoration: none;
    };
</style>