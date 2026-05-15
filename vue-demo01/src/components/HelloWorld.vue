<template>
  <div>test</div>
  <div v-bind:class="msg">test</div>
  <div v-bind:id="dynamicId" v-bind:class="dynamicClass">test</div>
  <div :id="dynamicId" :class="dynamicClass">test</div>

</template>

<script>
export default {
  data(){
    return{
      msg:"active",
      dynamicClass:"appleclass",
      dynamicId:"appleId"
    }
  }
}
</script>

<style>
.appleclass{
  color: red;
  font-size: 60px;
}
</style>