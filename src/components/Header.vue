<template>
  <header>
    
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
          link: '#',
          text: 'Home',
          active: true
        },
        {
          link: '#',
          text: 'Pages'
        },
        {
          link: '#',
          text: 'Program'
        },
        {
          link: '#',
          text: 'Tickets'
        },
        {
          link: '#',
          text: 'Speakers'
        },
        {
          link: '#',
          text: 'Papers'
        },
        {
          link: '#',
          text: 'Blog'
        },
        {
          link: '#',
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
  }

}

</style>
