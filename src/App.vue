<template>
  <div id="app">
    <child v-bind:title="title" v-on:update-title="title=$event"></child>
    <child :title.sync="title"></child>
    <child v-bind:title="title" v-on:update-title="title=$event"></child>
    <child v-bind:title="title" v-on:update-title="title=$event"></child>
  </div>
</template>

<script>
import Child from "./components/Child.vue";

export default {
  name: "App",
  components: {
    Child,
  },
  data(){
    return {
      title: 'myTitle'
    }
  }
};
</script>

<style>
</style>
