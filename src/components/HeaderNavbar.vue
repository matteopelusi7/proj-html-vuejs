<template>
  <li class="list-item">
    <a :class="element.active ? 'active' : '' " :href="element.link">{{ element.text }}</a>
  </li>
</template>

<script>
export default {
  name: 'HeaderNavbar',
  props: {
    element: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

.list-item {
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 700;
  color: $gray;

  a {
    cursor: pointer;
  }

  .active {
    color: $sienna;
    border-bottom: 2px solid $sienna;
  }

}

</style>
