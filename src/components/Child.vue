<template>
<div>
  <h2>{{ title }}</h2>
  <input v-on:input="$emit('update-title', $event.target.value)" v-bind:value="title" type="text"/>
</div>
</template>

<script>
export default {
    name: 'Child',
    props: ['title']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
