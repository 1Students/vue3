<template>
  <div>
      
      <span>我是子组件</span>
      <p><span>输入1</span>  <input type="text" v-model="name">  </p>
      <p><span>输入2</span>  <input type="text" v-model="usid" >  </p>
      <button @click="submit"> 登录  </button>
  </div>
</template>

<script>
export default {
  name:"child",
  data(){
    return{
      name:'',
      usid:'',
    }
  },
  created(){

  },
  methods:{
    submit(){
      console.log(2223)
      this.$emit("chi" ,this.name,this.usid )
    }
  }
}
</script>

<style>

</style>