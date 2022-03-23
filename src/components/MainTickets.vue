<template>
  <section>

    <div class="container">

      <div class="row row-title">
        <h3>Tickets</h3>
      </div>

      <div class="row row-box-ticket">

        <div class="box-ticket">
          <div class="ticket-header">
            <h3>One day pass</h3>
            <h4>Free</h4>
          </div>
          <div class="ticket-main">
            <p>One Day Access</p>
            <p>Coffee Break</p>
            <p>Lunch(International Buffet)</p>
            <p>Document Sheets</p>
            <p>50USD Voucher For Next Event</p>
          </div>
          <div class="ticket-footer">
            <h5>Book now</h5>
          </div>
        </div>

        <div class="box-ticket">
          <div class="ticket-header">
            <h3>Four Day passes</h3>
            <h4>750.00 USD</h4>
          </div>
          <div class="ticket-main">
            <p>Four Day Access</p>
            <p>Coffee Break</p>
            <p>Lunch(International Buffet)</p>
            <p>Document Sheets</p>
            <p class="price">100USD Voucher For Next Event</p>
          </div>
          <div class="ticket-footer">
            <h5>Book now</h5>
          </div>
          <div class="featured">
            <span>Featured!</span>
          </div>
        </div>

        <div class="box-ticket">
          <div class="ticket-header">
            <h3>Two Day Passes</h3>
            <h4>580.00 USD</h4>
          </div>
          <div class="ticket-main">
            <p>Two Day Access</p>
            <p>Coffee Break</p>
            <p>Lunch(International Buffet)</p>
            <p>Document Sheets</p>
            <p>70USD Voucher For Next Event</p>
          </div>
          <div class="ticket-footer">
            <h5>Book now</h5>
          </div>
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainTickets',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  background-image: url('../assets/img/ticket-bg.jpg');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  padding: 80px 0;

  .container {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    gap: 20px;
    
    .row-title {
      color: $white;
      text-transform: uppercase;
      font-size: 25px;
      padding-bottom: 35px;
    }

    .row-box-ticket {
      display: flex;
      gap: 20px;
    }

    .box-ticket {
      
      width: calc( 100% / 3 );
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 100%;
      background-color: #f9f9f9;
      position: relative;

      .ticket-header {
        text-align: center;
        background-color: #e9e9e9;
        text-transform: uppercase;
        padding: 25px 10px;

        h3 {
          padding-bottom: 5px;
        }

        h4 {
          color: $red;
        }

      }

      .ticket-main {
        background-color: #f9f9f9;
        padding: 25px 60px;
        color: $gray;
        line-height: 40px;
        text-align: center;
        font-size: 15px;
        font-style: italic;
      }

      .ticket-footer {
        background-color: $red;
        padding: 20px 40px;
        text-align: center;
        color: white;
        text-transform: uppercase;
        font-size: 15px;
      }

      .featured {
        transform: rotate(45deg);
        position: absolute;
        top: 16px;
        right: -25px;
        background-color: $red;
        color: $white;
        padding: 5px 25px;
        font-size: 14px;
      }

    }

  }

}

</style>
