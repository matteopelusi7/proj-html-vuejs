<template>
  <header id="home">
    
    <div class="container">

      <div class="row">

        <div class="logo-wrapper">
          <figure class="logo">
            <img src="../assets/img/logo.png" alt="">
          </figure>
        </div>

        <nav class="list-wrapper">
          <ul class="list-navbar">
            <HeaderNavbar v-for="(element, i) in navbar" :key="i" :element="element" /> 
            <i class="fa-solid fa-magnifying-glass"></i>
          </ul>
        </nav>

      </div>

    </div>

  </header>
</template>

<script>

import HeaderNavbar from './HeaderNavbar.vue'

export default {
  name: 'MainHeader',
  components: {
    HeaderNavbar
  },
  data() {
    return {
      navbar: [
        {
          link: '#home',
          text: 'Home',
          active: true
        },
        {
          link: '#about',
          text: 'Pages'
        },
        {
          link: '#program',
          text: 'Program'
        },
        {
          link: '#tickets',
          text: 'Tickets'
        },
        {
          link: '#speakers',
          text: 'Speakers'
        },
        {
          link: '#presentation',
          text: 'Papers'
        },
        {
          link: '#location',
          text: 'Blog'
        },
        {
          link: '#sponsor',
          text: 'Shortcodes'
        }
      ]
    }
  }
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

header {

  padding: 0 10px;

  .row {
    display: flex;
    align-items: center;
    padding: 30px 0;
  }

  .list-navbar {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
  }

  .list-wrapper {
    display: flex;
    justify-content: flex-end;
    flex-grow: 1;
  }

  i {
    color: $gray;
    cursor: pointer;
  }

}

</style>
