<template>
  <h3>条件渲染</h3>
  <div v-if="flag">can you see me?</div>
  <div v-if="type === 'A'">A</div>
  <div v-else-if="type === 'B'">B</div>
  <div v-else-if="type === 'C'">C</div>
  <div v-else>Not a/b/c</div>
  <div v-show="flag">show me?</div>
  
</template>

<script>
export default {
  data(){
    return{
      flag:true,
      type: "B"
    }
  }
}
</script>

