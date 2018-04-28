<template>

  <headroom>
    <header class="header">
      <div class="header__inner container">
        <Nav/>
      </div>
    </header>
  </headroom>

</template>

<script>
  import { headroom } from 'vue-headroom'
  import Nav from './Nav';

  export default {
    name: 'Header',
    data() {
      return {
        currentScrollY: 0,
        prevScrollY: 0,
        isPinned: true
      }
    },
    components: {
      Nav,
      headroom
    }
  }

</script>