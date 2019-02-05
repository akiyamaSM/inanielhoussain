<template>
  <div>
    <el-row v-loading="loading"
            element-loading-text="Please wait..."
      >
      <el-button @click="sayHello">Default</el-button>
      <el-button type="primary">Primary</el-button>
      <el-button type="success">Success</el-button>
      <el-button type="info">Info</el-button>
      <el-button type="warning">Warning</el-button>
      <el-button type="danger">Danger</el-button>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      loading: true
    };
  },
  created(){
    setTimeout(() => {
      this.loading = false
    }, 4000)
  },
  methods:{
    sayHello(){
      alert('Hola')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
