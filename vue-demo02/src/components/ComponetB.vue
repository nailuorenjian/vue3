<template>
    <h3>ComponetB</h3>
    <p>ComponetB:{{ title }}</p>
    <P>{{ onEvent('send data') }}</P>
</template>

<script>
export default{
    data(){
        return{
        }
    },
    props:{
        title:String,
        onEvent:Function
    }
}
</script>