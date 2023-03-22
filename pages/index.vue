<template>
  <div>
    <Menu></Menu>
  </div>
</template>

<script>
import Vue from 'vue'
import Menu from '../components/Menu.vue'

export default Vue.extend({
  name: 'IndexPage',
  components: { Menu },
})
</script>

<style>
:root {
  --color-primary: #ff6666;
}

body {
  background-color: black;
}
</style>
