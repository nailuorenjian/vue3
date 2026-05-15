<template>
    <div class="aside">
        <h3>Aside</h3>
        <Item/>
        <Item/>
        <Item/>
    </div>
</template>
  
<script>
import Item from './Item.vue'

export default{
  components:{
    Item
  }
}
</script>


<style scoped>
.aside{
    float: right;
    width: 33%;
    height: 500px;
    border: 5px solid #1234;
    text-align: center;
}
</style>

