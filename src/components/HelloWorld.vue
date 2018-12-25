<template>
  <div class="hello">
    <router-link to="login" class="login" @click="login">登录</router-link>
    <div class="regiset" @click="regiset">注册</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods:{
    login(){
      //console.log(9)
    },
    regiset(){
      this.$router.push({path:'/regiset'})
    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .hello{
    width: 100%;
    height: 100%;
    
  }
  .hello .login,.regiset{
      width: 100%;
      display: inline-block;
      text-decoration: none;
      border: solid 1px firebrick;
      height: 40px;
      border-radius: 20px;
      margin:10px 0;
      text-align: center;
      line-height: 40px;
    }
</style>
