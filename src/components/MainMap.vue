<template>
  <section id="map">

    <div class="img-wrapper">
      <img src="../assets/img/vt (23).png" alt="">
      <img src="../assets/img/vt (17).png" alt="">
      <img src="../assets/img/vt (11).png" alt="">
      <img src="../assets/img/vt (1).png" alt="">
      <img src="../assets/img/vt (5).png" alt="">
      <img src="../assets/img/vt (4).png" alt="">
      <img src="../assets/img/vt (9).png" alt="">
      <img src="../assets/img/vt (20).png" alt="">
      <img src="../assets/img/vt (24).png" alt="">
      <img src="../assets/img/vt (19).png" alt="">
      <img src="../assets/img/vt (13).png" alt="">
      <img src="../assets/img/vt (12).png" alt="">
      <img src="../assets/img/vt (2).png" alt="">
      <img src="../assets/img/vt.png" alt="">
      <img src="../assets/img/vt (3).png" alt="">
      <img src="../assets/img/vt (15).png" alt="">
      <img src="../assets/img/vt (18).png" alt="">
      <img src="../assets/img/vt (25).png" alt="">
      <img src="../assets/img/vt (22).png" alt="">
      <img src="../assets/img/vt (16).png" alt="">
      <img src="../assets/img/vt (8).png" alt="">
      <img src="../assets/img/vt (10).png" alt="">
      <img src="../assets/img/vt (6).png" alt="">
      <img src="../assets/img/vt (7).png" alt="">
      <img src="../assets/img/vt (14).png" alt="">
      <img src="../assets/img/vt (21).png" alt="">
      <img src="../assets/img/vt (26).png" alt="">
    </div>

    <div class="box-map">
      <p>Map</p>
      <p>Satellite</p>
    </div>

    <div class="box-google">
      <figure>
        <img src="../assets/img/google4.png" alt="">
      </figure>
    </div>

    <div class="box-person">
      <figure>
        <svg xmlns="http://www.w3.org/2000/svg" width="23" height="38" viewBox="0 0 23 38">
        <path d="M16.6,38.1h-5.5l-0.2-2.9-0.2,2.9h-5.5L5,25.3l-0.8,2a1.53,1.53,0,0,1-1.9.9l-1.2-.4a1.58,1.58,0,0,1-1-1.9v-0.1c0.3-.9,3.1-11.2,3.1-11.2a2.66,2.66,0,0,1,2.3-2l0.6-.5a6.93,6.93,0,0,1,4.7-12,6.8,6.8,0,0,1,4.9,2,7,7,0,0,1,2,4.9,6.65,6.65,0,0,1-2.2,5l0.7,0.5a2.78,2.78,0,0,1,2.4,2s2.9,11.2,2.9,11.3a1.53,1.53,0,0,1-.9,1.9l-1.3.4a1.63,1.63,0,0,1-1.9-.9l-0.7-1.8-0.1,12.7h0Zm-3.6-2h1.7L14.9,20.3l1.9-.3,2.4,6.3,0.3-.1c-0.2-.8-0.8-3.2-2.8-10.9a0.63,0.63,0,0,0-.6-0.5h-0.6l-1.1-.9h-1.9l-0.3-2a4.83,4.83,0,0,0,3.5-4.7A4.78,4.78 0 0,0 11 2.3H10.8a4.9,4.9,0,0,0-1.4,9.6l-0.3,2h-1.9l-1,.9h-0.6a0.74,0.74,0,0,0-.6.5c-2,7.5-2.7,10-3,10.9l0.3,0.1,2.5-6.3,1.9,0.3,0.2,15.8h1.6l0.6-8.4a1.52,1.52,0,0,1,1.5-1.4,1.5,1.5,0,0,1,1.5,1.4l0.9,8.4h0Zm-10.9-9.6h0Zm17.5-.1h0Z" style="fill:#333;opacity:0.7;isolation:isolate"/>
        <path d="M5.9,13.6l1.1-.9h7.8l1.2,0.9" style="fill:#ce592c"/>
        <ellipse cx="10.9" cy="13.1" rx="2.7" ry="0.3" style="fill:#ce592c;opacity:0.5;isolation:isolate"/>
        <path d="M20.6,26.1l-2.9-11.3a1.71,1.71,0,0,0-1.6-1.2H5.7a1.69,1.69,0,0,0-1.5,1.3l-3.1,11.3a0.61,0.61,0,0,0,.3.7l1.1,0.4a0.61,0.61,0,0,0,.7-0.3l2.7-6.7,0.2,16.8h3.6l0.6-9.3a0.47,0.47,0,0,1,.44-0.5h0.06c0.4,0,.4.2,0.5,0.5l0.6,9.3h3.6L15.7,20.3l2.5,6.6a0.52,0.52,0,0,0,.66.31h0l1.2-.4a0.57,0.57,0,0,0,.5-0.7h0Z" style="fill:#fdbf2d"/>
        <path d="M7,13.6l3.9,6.7,3.9-6.7" style="fill:#cf572e;opacity:0.6;isolation:isolate"/>
        <circle cx="10.9" cy="7" r="5.9" style="fill:#fdbf2d"/>
        </svg>
      </figure>
    </div>

    <div class="box-plus">
      <i class="fa-solid fa-plus"></i>
      <i class="fa-solid fa-minus"></i>
    </div>

  </section>
</template>

<script>
export default {
  name: 'MainMap',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  position: relative;

  .img-wrapper {
    display: flex;
    flex-wrap: wrap;
  }
  
  img {
    display: block;
    width: calc( 100% / 9)
  }

  .box-google {

    img {
      width: 80px;
      height: 35px;
      position: absolute;
      bottom: 10px;
      left: 10px;
    }

  }

  .box-person {
    position: absolute;
    bottom: 120px;
    right: 10px;
    background-color: $white;
    padding: 5px;
    cursor: pointer;
  }

  .box-plus {
    position: absolute;
    bottom: 20px;
    right: 10px;
    display: flex;
    flex-direction: column;
    color: $gray;

    i {
      background-color: $white;
      padding: 7px 8px;
      gap: 10px;
      cursor: pointer;
    }
  }

  .box-map {
    position: absolute;
    top: 10px;
    left: 10px;
    display: flex;

    p {
      background-color: $white;
      padding: 7px 12px;
      gap: 10px;
      cursor: pointer;
    }

    p:first-child {
      border-right: 2px solid $cloud;
    }

    p:last-child {
      color: $gray;
    }
  }

}

</style>
