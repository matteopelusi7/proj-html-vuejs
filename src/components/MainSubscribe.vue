<template>
  <section id="subscribe">

    <div class="container">

      <div class="row">

        <div class="countdown">
          <div class="box-count">
            <p class="num-count">3339</p>
            <p class="type-count">Days</p>
          </div>
          <div class="box-count">
            <p class="num-count">7</p>
            <p class="type-count">Hours</p>
          </div>
          <div class="box-count">
            <p class="num-count">28</p>
            <p class="type-count">mins</p>
          </div>
          <div class="box-count">
            <p class="num-count">17</p>
            <p class="type-count">secs</p>
          </div>
        </div>
        <div class="subscribe">
          <p>Subscribe for updates</p>
        </div>
        <div class="form">
          <input type="text" placeholder="Please fill your email">
          <button>Subscribe</button>
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainSubscribe',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  background-image: url('../assets/img/coutdown-bg1.jpg');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  padding: 80px 10px;

  .row {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    gap: 40px;

    .subscribe {
      text-transform: uppercase;
      font-size: 20px;
      font-weight: 600;
    }

    .form {

      input {
        width: 300px;
        border: none;
        padding: 15px 10px;
        border-radius: 2px;
        margin-right: 10px;
      }

      button {
        color: $white;
        background-color: #f62b0a;
        border: none;
        text-transform: uppercase;
        padding: 15px 25px;
        border-radius: 3px;
        font-weight: 600;
        cursor: pointer;
        margin-top: 5px;
      }

    }

    .countdown {
      display: flex;
      gap: 15px;

      .box-count {
        color: $white;
        background-color: $black;
        opacity: 0.6;
        padding: 30px;
        text-align: center;
        border-radius: 5px;

        .num-count {
          font-size: 40px;
          font-weight: 700;
        }

        .type-count {
          text-transform: uppercase;
          font-size: 12px;
        }

        &:first-child {
          opacity: 0.8;
        }

      }

    }

  }

}

</style>
