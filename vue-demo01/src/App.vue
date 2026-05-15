<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import IfDemo from './components/IfDemo.vue'
import VforList from './components/VforList.vue'
import KeyDemo from './components/KeyDemo.vue'
import EventDemo from './components/EventDemo.vue'
import EventDemo6 from './components/EventDemo6.vue'
import watchDemo from './components/watchDemo.vue'
import model from './components/model.vue'

</script>

<template>
  <header>
    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
    <IfDemo></IfDemo>
    <VforList></VforList>
    <KeyDemo></KeyDemo>
    <EventDemo></EventDemo>
    <EventDemo6></EventDemo6>
    <watchDemo></watchDemo>
    <model></model>
  </header>
</template>


 