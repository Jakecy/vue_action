<!—把button.vue和title.vue引入到App.vue文件中作为子组件使用-->


<template>
   <div>
     <!--使用子组件-->
     <v_title title="Vue组件化"></v_title>
     <v_button @click="handleClick">点击按钮</v_button>
   </div>

</template>


<script>
   //引入组件
   import  v_title from './components/title.vue';
   import  v_button from './components/button.vue';


  export default {

      components:{
        v_title: v_title,
        v_button: v_button
      },
    methods: {
        handleClick(e){
          console.log(e);
        }
    }
  }
</script>

<style scoped>
  div{
        color: #f60;
        font-size: 24px;
  }
</style>
