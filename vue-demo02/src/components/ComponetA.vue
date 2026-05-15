<template>
    <h3>ComponetA</h3>
    <ComponetB title="ComponetA 表题" :onEvent="dataFn"/>
    <p>{{ message }}</p>
</template>


<script>
import ComponetB from './ComponetB.vue'

export default{
    data(){
        return{
            message:""
        }
    },
    components:{
        ComponetB
    },
    methods:{
        dataFn(data){
            console.log(data);
            this.message=data
        }
    }
}
</script>