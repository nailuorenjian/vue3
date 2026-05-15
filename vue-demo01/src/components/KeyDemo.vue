<template>
  <h3>V-for</h3>
  <P v-for="(item, index) in names" :key="index">{{ item }}</P>
  <button @click="count++">Add 1</button>
  <p>Count is: {{ count }}</p>
</template>

<script>

export default {
  data(){
    return{
      names:["test4", "test5", "test6"],
      count:0
    }
  }
}
</script>

