<template>
    <h3>Parent</h3>
    <!-- <Child title="Parent data"/> -->
    <Child :title="message" :age="age" @someEvent="getHandler"/>

</template>

<script>
import Child from './Child.vue'

export default{
  components: { Child },
    data(){
        return{
            message:"parent data",
            age:20
        }
    },
    components:{
        Child
    },
    methods:{
        getHandler(data){
            console.log("event child",data);
            this.message = data;
        }
    }
}
</script>