<template>

  <div class="row">
    <div class="box-footer">
      <h4 class="title-footer">About Us</h4>
      <p class="description-footer">Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
      <div class="icon-footer">
        <i class="fa-brands fa-facebook-square"></i>
        <i class="fa-brands fa-twitter-square"></i>
        <i class="fa-brands fa-linkedin"></i>
        <i class="fa-brands fa-google-plus-square"></i>
        <i class="fa-brands fa-pinterest-square"></i>
        <i class="fa-solid fa-square-share-nodes"></i>
      </div>
    </div>
    <div class="box-footer">
      <h4 class="title-footer">Recent News</h4>
      <ul class="description-footer">
        <li class="list" v-for="(item, i) in listItem" :key="i">
          <i class="fa-solid fa-caret-right"></i>
          {{ item.text }}
        </li>
      </ul>
    </div>
    <div class="box-footer">
      <h4 class="title-footer">Get your seat!</h4>
      <p class="description-footer">Book for your seat before it's too rate. We provide variety of ticket options.</p>
      <button class="button"><a href="#tickets">Check out tickets!</a></button>
    </div>
    <div class="box-footer">
      <h4 class="title-footer">Gallery from last year</h4>
      <ul class="img-wrapper">
        <li class="img-list" v-for="(img, i) in imgItem" :key="i">
          <img :src="img.img" alt="">
        </li>
      </ul>
    </div>
  </div>

</template>

<script>
export default {
  name: 'FooterList',
  props: {
    listItem: Array,
    imgItem: Array
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

.box-footer {

  width: calc( (100% / 4) - 20px);

  .title-footer {
    text-transform: uppercase;
    padding-bottom: 20px;
  }

  i {
    cursor: pointer;
  }

  .description-footer {
    color: $gray;
    padding-bottom: 20px;
  }

  .icon-footer {
    display: flex;
    gap: 20px;
    font-size: 21px;
  }

  .button {
    color: $white;
    background-color: $red;
    border: none;
    text-transform: uppercase;
    padding: 10px 20px;
    font-size: 12px;
    border-radius: 3px;
    font-weight: 600;
    cursor: pointer;
    margin-top: 5px;
  }

  .list {
    text-transform: uppercase;
    line-height: 22px;
    font-size: 13px;

    i {
      padding-right: 5px;
    }

  }

  .img-wrapper {
    display: flex;
    flex-wrap: wrap;
    gap: 7px;
  }

  .img-list {
    width: calc( (100% / 4) - 7px);
  }

}

@media all and (max-width: 770px) {

  .box-footer {
    width: 50%;
  }

}

</style>
