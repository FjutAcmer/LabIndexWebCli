<template>
  <div class="home-body">
    <el-row :gutter="40">
      <el-col :span="8"
              v-for="item in this.pageData"
              :key="item">
        <el-card class="page-card"
                 shadow="hover">
          <div slot="header">
            <span class="des-font">{{item.name}}</span>
          </div>
          <el-image class="des-image"
                    :src="item.picUrl">
          </el-image>
          <el-link type="primary"
                   :href="item.url"
                   target="_blank">{{item.url}}</el-link>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data () {
    return {
      pageData: [
        {
          name: '一码当先在线编程系统（重构版）',
          url: 'http://acm.fjutcoder.com',
          picUrl: require('../assets/image/cf.jpg')
        },
        {
          name: '一码当先在线编程系统（旧版）',
          url: 'http://oj.fjutcoder.com',
          picUrl: require('../assets/image/cf.jpg')
        },
        {
          name: 'GitLab',
          url: 'http://gitlab.fjutcoder.com',
          picUrl: require('../assets/image/gitlab.jpg')
        },
        {
          name: 'API接口',
          url: 'http://api.fjutcoder.com',
          picUrl: require('../assets/image/api.jpg')
        },
        {
          name: 'Tomcat后台',
          url: 'http://tomcat.fjutcoder.com',
          picUrl: require('../assets/image/tomcat.jpg')
        },
        {
          name: '管理员后台',
          url: 'http://admin.fjutcoder.com',
          picUrl: require('../assets/image/admin-fun.jpg')
        }
      ]
    }
  },
  methods: {
  }
}
</script>

<style scoped>
.home-body {
  width: 100%;
  min-height: 100%;
  margin: auto;
  background-color: #ffffff;
}

.page-card {
  height: 200px;
  margin-bottom: 20px;
  /* background-color: yellow; */
}

.des-image {
  width: 100px;
  height: 100px;
}
</style>
