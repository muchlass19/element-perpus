<template>
    <div>     
        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect"
        background-color="#0D78E7" text-color="#fff" active-text-color="#fff">
          <el-menu-item index="1">Perpustakaan</el-menu-item>
          <el-menu-item index="2">Beranda</el-menu-item>
          <el-menu-item index="3">Daftar Buku</el-menu-item>
          <el-submenu index="4">
            <template slot="title">Akun</template>
            <el-menu-item index="4-1">Profil</el-menu-item>
            <el-menu-item index="4-2">Keluar</el-menu-item>
          </el-submenu>
          <el-menu-item index="5" class="el-icon-search">
            Search
            <input style="border: none; border-radius: 3px; padding: 4px 10px" type="text">
          </el-menu-item>
        </el-menu>
    </div>
</template>
<script>
  export default {
    data() {
      return {
        activeIndex: '1',
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