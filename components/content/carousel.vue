<template>
    <el-carousel :interval="4000" type="card" height="300px">
        <el-carousel-item>
          <img src="https://www.infobdg.com/v2/wp-content/uploads/2017/07/341-library.jpg" style="width: 800px; height: 300px;" alt="">
        </el-carousel-item>
        <el-carousel-item>
            <img src="https://awsimages.detik.net.id/visual/2019/05/01/35344e00-03ef-4cb5-9c22-59a54a06ec5d_169.jpeg?w=360&q=90" style="width: 800px; height: 300px" alt="">
        </el-carousel-item>
        <el-carousel-item>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSNZpE0qGhykUo6YtBcFR2qj6AA2TRobx7opwIAsL9ArbbaahiQ" style="width: 800px; height: 300px" alt="">
        </el-carousel-item>
    </el-carousel>
</template>

<script>
export default {

}
</script>

<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  };

  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  };

  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  };
</style>