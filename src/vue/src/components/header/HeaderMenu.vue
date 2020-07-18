<template>
<ul class="menu">
  <li v-for="item in menu" :key="item.name">
    <a :href="item.url">{{ item.name }}</a>
  </li>
</ul>
</template>

<script>
export default {
  name: 'HeaderMenu',
  props: {
    menu: Array
  }
}
</script>

<style>

</style>