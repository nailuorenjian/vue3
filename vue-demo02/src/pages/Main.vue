<template>
    <div class="main">
        <h3>Main</h3>
        <Article/>
        <Article/>
    </div>
</template>


<script>
import Article from './Article.vue'

export default{
  components:{
    Article
  }
}
</script>



<style scoped>
.main{
    float: left;
    width: 65%;
    height: 500px;
    border: 5px solid #1234;
    text-align: center;
}
</style>

