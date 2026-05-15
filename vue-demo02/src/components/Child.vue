<template>
    <h3>Child</h3>
    <p>{{ title }}</p>
    <p>{{ age }}</p>
    <button @click="clickEvent">传递参数</button>

</template>

<script>
export default{
    data(){
        return{
            age:{
                type:Number,
                default:0
            }
        }
    },
    //父传子 传递数据
    props:["title","age"],
    methods:{
        clickEvent(){
            // 子传父
            this.$emit("someEvent","child data")
        }
    }
}
</script>