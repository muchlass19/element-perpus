<template>
  <div>
    <Navbar />
    <el-container>
      <el-main>
        <el-table :data="buku" :key="buku.id" stripe style="width: 80%;" border>
          <el-table-column prop="id" label="Id">
          </el-table-column>
          <el-table-column prop="nama" label="Nama">
          </el-table-column>
          <el-table-column prop="kategori" label="Kategori">
          </el-table-column>
          <el-table-column prop="penulis" label="Penulis"> </el-table-column>
        </el-table>
        <el-footer>
          <div class="block">
            <el-pagination
              @size-change="handleSizeChange"
              @current-change="handleCurrentChange"
              :current-page.sync="currentPage4"
              :page-sizes="[10, 20, 30, 40]"
              :page-size="20"
              layout="total, sizes, prev, pager, next"
              :total="400"
            >
            </el-pagination>
          </div>
        </el-footer>
      </el-main>
    </el-container>
  </div>
</template>

<script>
import Navbar from "~/components/content/navside.vue";
export default {
  components: {
    Navbar
  },
  data() {
    return {
      buku: [],
      currentPage1: [],
      currentPage2: [],
      currentPage3: [],
      currentPage4: []
    };
  },
  mounted() {
    this.getData();
  },
  methods: {
    async getData() {
      try {
        const res = await this.$axios.get("http://localhost:3001/buku");
        this.buku = res.data;
      } catch (err) {}
    }
  },
  handleSizeChange(val) {
    console.log(`${val} items per page`);
  },

  handleCurrentChange(val) {
    console.log(`current page: ${val}`);
  }
};
</script>

<style>

</style>