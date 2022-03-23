<template>
  <footer>

    <section class="footer-main">

      <div class="container">

        <div class="row">
          
          <FooterList :listItem="listItem" :imgItem="imgItem"/>

        </div>

      </div>

    </section>

    <section class="footer-final">

      <div class="container">

        <div class="row">
          <p>&copy; Copyright GoodLayers All Right Reserved</p>
          <p>About Us | Accomodation | Call For Paper | Contact Us</p>
        </div>

      </div>

    </section>

  </footer>
</template>

<script>

import FooterList from './FooterList.vue'

export default {
  name: 'FooterContent',
  components: {
    FooterList
  },
  data () {
    return {
      listItem: [
        {
          text: 'Sem porta mollis parturient'
        },
        {
          text: 'Nullam lorem mattis purus'
        },
        {
          text: 'Nibh sem sit ullamcorper'
        },
        {
          text: 'Donec luctus imperdiet'
        },
        {
          text: 'Magna pars studiorum'
        },
      ],
      imgItem: [
        {
          img: require('../assets/img/photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (1).jpg')
        },
        {
          img: require('../assets/img/photodune-8523683-speaker-at-business-convention-and-present.jpg')
        },
        {
          img: require('../assets/img/photodune-6745579-modern-creative-man-relaxing-on-workspace-.jpg')
        },
        {
          img: require('../assets/img/photodune-8522811-speaker-at-business-conference-and-present (1).jpg')
        },
        {
          img: require('../assets/img/photodune-8797753-multiethnic-people-with-startup-business-t (1).jpg')
        },
        {
          img: require('../assets/img/card04-150x150.jpg')
        },
        {
          img: require('../assets/img/photodune-6745606-man-wristwatch-calendar-key-and-glasses-on.jpg')
        },
        {
          img: require('../assets/img/photodune-6745585-modern-creative-workspace-m-150x150.jpg')
        },
        {
          img: require('../assets/img/6426608875_186070f8ca_o-150x150.jpg')
        },
        {
          img: require('../assets/img/card01-150x150.jpg')
        },
        {
          img: require('../assets/img/13349065283_64d09b067c_o-150x150.jpg')
        },
        {
          img: require('../assets/img/photodune-8795110-overhead-of-essentials-denim-clothes-m-150.jpg')
        },
      ]
    }
  }
}

</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

footer {

  .footer-main {
    padding: 50px 0;
    background-color: #212121;

    .row {
      display: flex;
      justify-content: center;
      gap: 40px;
      color: $white;
    }

  }

  .footer-final {
    padding: 35px 0;
    background-color: $black;
    color: $gray;

    .row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 14px;
    }
  }

}

</style>
