<template>
  <h3>事件修饰符</h3>
  <a @click="clickHandle" href="ciao.party">豌豆公主</a>
  <button @click="addCount">Add 1</button>
  <p>Count is: {{ count }}</p>
  <div @click="clickDiv">
  <p @click="clickP">ppp</p></div>
</template>

<script>

export default {
  data(){
    return{
      count:0
    }
  },
  methods:{
    addCount(){
      this.count++;
    },
    clickHandle(e){
      //阻止默认事件
      e.preventDefault(); //等于@click.prevent
      console.log("clicked");
    },
    clickDiv(){
      console.log("div clicked");
    },
    clickP(){
      console.log("click p");
    }
  }
}
</script>

