<template>
  <div id="app">
    <el-container>
      <el-header>
        <Header />
      </el-header>
      <el-main>
        <router-view />
      </el-main>
      <el-footer>
        <Footer />
      </el-footer>
    </el-container>
  </div>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #f2f6fc;
}

.el-header {
  width: 80%;
  margin: auto;
  height: 50px;
}

.el-main {
  width: 80%;
  margin: auto;
}

.el-footer {
  width: 80%;
  margin: auto;
  height: 50px;
}
</style>
