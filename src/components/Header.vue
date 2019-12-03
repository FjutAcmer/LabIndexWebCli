<template>
  <div id="header-body">
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b"
    >
      <el-menu-item index="1">FJUT 515创新实验室</el-menu-item>
      <el-menu-item index="2"></el-menu-item>
      <el-menu-item index="3"></el-menu-item>
      <el-menu-item index="4"></el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  data () {
    return {
      activeIndex: '1'
    }
  },
  methods: {
    handleSelect () { }
  }
}
</script>

<style scoped>
.header-body {
  width: 100%;
  height: 100%;
}
</style>
