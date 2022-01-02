<template>
  <div id="Javascript">
      <p>{{lang}}</p>
      <button @click="tab='Vue'">Vue</button>
      <button @click="tab='React'">React</button>
      <button @click="tab='Angular'">Angular</button>
      <component :is="tab"></component>
  </div>
</template>

<script>
import Vue from './Vue.vue';
import React from './React.vue';
import Angular from './Angular.vue';
export default {
    name: 'Javascript',
    components: {
        Vue,
        React,
        Angular
    },
    data(){
        return{
            lang: 'javascript',
            tab: 'Vue'
        }
    }
}
</script>

<style>

</style>