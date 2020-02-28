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
          name: '一码当先 | CodingFirst',
          url: 'https://acm.fjutcoder.com',
          picUrl: require('../assets/image/cf.jpg')
        },
        {
          name: '实验室GIT | GitLab',
          url: 'https://gitlab.fjutcoder.com',
          picUrl: require('../assets/image/gitlab.jpg')
        },
        {
          name: '服务端接口 | API',
          url: 'https://api.fjutcoder.com',
          picUrl: require('../assets/image/api.jpg')
        },
        {
          name: '管理员后台 | Admin',
          url: 'https://admin.fjutcoder.com',
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
  min-height: 500px;
  margin: auto;
  background-color: #f2f6fc;
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
