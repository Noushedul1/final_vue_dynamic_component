<template>
 <div id="App">
   <button @click="tab='Javascript'">Javascript</button>
   <button @click="tab='Php'">Php</button>
   <button @click="tab='Sass'">Sass</button>
   <component :is="tab"></component>
 </div>
</template>

<script>
import Javascript from './components/Javascript.vue';
import Php from './components/Php.vue';
import Sass from './components/Sass.vue';
export default {
  name: 'App',
  components: {
    Javascript,
    Php,
    Sass
  },
data(){
  return{
    tab: 'Javascript'
  }
}
}
</script>

<style>

</style>