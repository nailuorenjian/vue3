<template>
  <h3>监听器</h3>
 
  <p>{{ message }}</p>
  <button @click="updateHandle">修改数据</button>
  
</template>

<script>

export default {
  data(){
    return{
      message:"hello"
    }
  },
  methods:{
    updateHandle(){
      this.message = "word"
    }
  },
  watch:{
    message(newValue, oldValue){
      console.log(newValue,oldValue)
    }
  }
}
</script>

