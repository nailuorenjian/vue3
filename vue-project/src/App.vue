
<template>
  <!--3:显示组件-->
  <MyComponentVue/>
</template>

<script>
//1:引入组件
import MyComponentVue from './components/MyComponent.vue'

export default{
  //2:注入组件
  components:{
    MyComponentVue
  }
}
</script>

<style>
/* <style scoped> scoped 只在当前组件中生效 */
</style>

