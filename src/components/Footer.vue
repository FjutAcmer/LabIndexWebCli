<template>
  <div class="footer-body">
    <span class="backup-span" @click="toBeian()">闽ICP备19024997号</span>
    <br />
    <span class="power-span">Power by ©福建工程学院-信息科学与工程学院-515创新实验室</span>
  </div>
</template>

<script>
export default {
  methods: {
    toBeian () {
      window.open('http://www.beian.miit.gov.cn/')
    }
  }
}
</script>

<style scoped>
.footer-body {
  width: 100%;
  min-height: 65px;
  background-color: rgb(84, 92, 100);
}

.backup-span {
  cursor: pointer;
  color: white;
  line-height: 30px;
}

.power-span {
  margin: 5px;
  color: rgb(255, 208, 75);
}
</style>
