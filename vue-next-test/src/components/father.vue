<template>
  <div>
       <div>
      
      <span>我是父组件组件</span>
    
     
    <div>我发送给第一个组件的信息是:{{msgkk}}</div>
      <ChildOne :adke="msgkk" /> 
       <h2>{{ title }}</h2>
  </div>
  </div>
</template>

<script>
// import ChildOne from "./HelloWorld"
export default {
    name:'father',
    props: ['title'],
 data(){
    return{
      name:'',
      usid:'',
      msgkk:"我是你ather",
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