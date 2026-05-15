<template>
    <h3>Mains</h3>
    <p>search info:{{ search }}</p>
    <SerachComponent @searchEvent="getSearch"/>
</template>

<script>
import SerachComponent from './SerachComponent.vue'

export default{
    data(){
        return{
            search:""
        }
    },
    components:{
        SerachComponent
    },
    methods:{
        getSearch(data){
            this.search = data
        }
    }
   
}
</script>