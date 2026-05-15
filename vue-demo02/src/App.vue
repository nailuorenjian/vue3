<template>
  <keep-alive>
    <component :is="tabCompoent"></component>
  </keep-alive>
  <button @click="changeHandle">switch componentC&D</button>

  <ComponetA/>
  <Mains/>
  <!-- <SerachComponent/> -->
  <Parent/>
  <Header/>
  <Main/>
  <Aside/>

</template>


<script>
import ComponetC from './components/ComponetC.vue'
import ComponetD from './components/ComponetD.vue'

import ComponetA from './components/ComponetA.vue'
import Header from './pages/Header.vue'
import Main from './pages/Main.vue'
import Mains from './components/Mains.vue'
import SerachComponent from './components/SerachComponent.vue'

import Aside from './pages/Aside.vue'
import Parent from './components/Parent.vue'


export default{
  components:{
    Header,
    Main,
    Aside,
    Parent,
    Mains,
    SerachComponent,
    ComponetA,
    ComponetC,
    ComponetD
  },
  data(){
    return{
      tabCompoent:"ComponetC"
    }
  },
  methods:{
    changeHandle(){
      this.tabCompoent = this.tabCompoent == "ComponetC" ? "ComponetD" : "ComponetC"
    }
  }
}
</script>

<style scoped>

</style>
