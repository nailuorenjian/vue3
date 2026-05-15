<template>
  <h3>V-for</h3>
  <P v-for="item in names">{{ item }}</P>
  
</template>

<script>

export default {
  data(){
    return{
      names:["test1", "test2", "test3"]
    }
  }
}
</script>

