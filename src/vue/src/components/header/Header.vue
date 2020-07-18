<template>
  <div class="header">
    <HeaderMenu :menu="menu" />
    <HeaderCart />
  </div>
</template>

<script>
import HeaderMenu from './HeaderMenu.vue';
import HeaderCart from './HeaderCart.vue';
export default {
  name: 'Header',
  components: {
    HeaderMenu,
    HeaderCart
  },
  data () {
    return {
      menu: [
        { name: 'Hakkimizda', url: '/hakkimizda' },
        { name: 'Urunlerimiz', url: '/urunlerimiz' },
        { name: 'Iletisim', url: '/iletisim' }
      ]
    }
  }
}
</script>

<style>
  .menu {
    display: flex;
  }
  .menu li {
    padding: 10px;
  }
</style>