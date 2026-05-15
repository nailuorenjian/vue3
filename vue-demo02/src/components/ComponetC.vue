<template>
    <h3>ComponetC</h3>
    <p>{{ message }}</p>
    <button @click="update">switch data</button>
</template>


<script>

export default{
    data(){
        return{
            message:"old data"
        }
    },
    methods:{
        update(){
            this.message = "new data"
        }
    }
}
</script>