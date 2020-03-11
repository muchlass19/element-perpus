<template>
  <div>
    <NavSide></NavSide>
      <el-carousel :interval="4000" type="card" height="500px">
        <el-carousel-item>
          <img src="https://www.ecopetit.cat/wpic/mpic/4-42716_fondos-de-pantalla-4k.jpg" alt="">
      </el-carousel-item>
      <el-carousel-item>
          <img src="https://www.ecopetit.cat/wpic/mpic/4-42716_fondos-de-pantalla-4k.jpg" alt="">
      </el-carousel-item>
      <el-carousel-item>
          <img src="https://www.ecopetit.cat/wpic/mpic/4-42716_fondos-de-pantalla-4k.jpg" alt="">
      </el-carousel-item>
  </el-carousel>
  </div>
</template>

<script>
import NavSide from '~/components/navside.vue'
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo,
    NavSide
  }
}
</script>

<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
</style>
