<template>

  <nav class="nav" :class="{ 'is-open': isOpen }">


    <!-- burger -->
    <div class="nav__burger">
      <button type="button" class="burger btn" @click.prevent="toggleMenu">
        <span class="burger__inner"></span>
      </button>
    </div>


    <!-- main -->
    <div class="nav__main">
      <ul class="nav__list">
        <li class="nav__item" v-for="link, index in links" :key="index">
          <a href="#" class="nav__link link">{{ link }}</a>
        </li>
      </ul>
    </div>


    <!-- overlay -->
    <div class="nav__overlay" @click="toggleMenu"></div>

  </nav>

</template>

<script>

  export default {
    name: 'Nav',
    data() {

      return {
        isOpen: false,
        links: ['Home', 'About us', 'Contact us']
      }

    },
    methods: {
      toggleMenu() {
        this.isOpen = !this.isOpen;
      }
    }
  }

</script>