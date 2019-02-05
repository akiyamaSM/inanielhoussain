<template>
  <div>
      <el-row class="header">
          <el-col :span="12" class="text">
              <el-carousel indicator-position="none" arrow="never" :interval="3000">
                  <el-carousel-item>
                      <span class="big-title">
                          You think <br>
                          You Want <br>
                          <strong>We Make</strong>
                      </span>
                  </el-carousel-item>
                  <el-carousel-item>
                      <span class="big-title">
                          You think2 <br>
                          You Want3 <br>
                          <strong>We Make</strong>
                      </span>
                  </el-carousel-item>
              </el-carousel>
          </el-col>
          <el-col :span="12">
              <img src="/img/me.png" alt="me">
          </el-col>

      </el-row>
  </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    .header{
        background-color: #409EFF;
        height: 600px;
        font-family: "Helvetica Neue", sans-serif;
    }

    .header .text{
        height: 100%;
    }

    img{
        position: absolute;
        right: 0;
        bottom: 0;
        height: 500px;
    }

    .big-title{
        font-size: 100px;
        color: white;
    }
</style>