<template>
  <div style="text-align: center;">
    <el-menu :default-active="activeIndex" @select="handleSelect">
        <el-badge class="item">
          <el-button size="large">Sejarah</el-button>
        </el-badge>
        <el-badge class="item">
          <el-button size="large">Komputer</el-button>
        </el-badge>
        <el-badge class="item">
          <el-button size="large">Pendidikan</el-button>
        </el-badge>
        <el-badge class="item">
          <el-button size="large">Ekonomi</el-button>
        </el-badge>
        <el-badge class="item">
          <el-button size="large">Bahasa</el-button>
        </el-badge>
        <el-badge class="item">
          <el-button size="large">Anak - Anak</el-button>
        </el-badge>
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

<style>

</style>