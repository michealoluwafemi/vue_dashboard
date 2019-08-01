<template>
  <div class="padded">
    <img src="../assets/icons/student-fee.png" />
    <span class="title">Student Fees</span>
    <div class="st-f">
      <div class="box">
        <router-link to="/invoiced">
          <div class="img-bg div-primary">
            <img src="../assets/icons/approve-invoice.png" title="invoiced" alt="invoiced"/>
          </div>
          <div>
            <span>invoiced</span>
            <p class="c-text">#2,300,000.00</p>
          </div>
        </router-link>
      </div>
      <div class="box">
        <router-link to="/recieved">
          <div class="img-bg div-success">
            <img src="../assets/icons/money.png" title="recieved" alt="recieved"/>
          </div>
          <div>
            <span>recieved</span>
            <p class="c-text">#1,700,000.00</p>
          </div>
        </router-link>
      </div>
      <div class="box">
        <router-link to="/pending">
          <div class="img-bg div-warning">
            <img src="../assets/icons/sand-clock.png" title="pending" alt="pending"/>
          </div>
          <div>
            <span>pending</span>
            <p class="c-text">#6,000,000.00</p>
          </div>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'stuFees',
  props: {

  },
  data() {
    return {
      cardLists: [
        {
          imgUrl: "../assets/icons/approve-invoice.png",
          title: "invoiced",
          amt: "#2,300,000.00",
          cardClass: "img-bg div-primary"
        },
        {
          imgUrl: "../assets/icons/approve-invoice.png",
          title: "recieved",
          amt: "#1,700,000.00",
          cardClass: "img-bg div-success"
        },
        {
          imgUrl: "../assets/icons/approve-invoice.png",
          title: "pending",
          amt: "#6,000,000.00",
          cardClass: "img-bg div-warning"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .padded {
    margin-top: 20px;
  }
  .padded .title {
    margin-left: 14px;
    text-transform: uppercase;
    font-family: Khula;
    font-style: normal;
    font-weight: normal;
    font-size: 10px;
    letter-spacing: 1px;
    color: #3B3B3B;
  }
  .st-f {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 20px;
    overflow: auto;
    margin-top: 9px;
  }
  .st-f .box {
    height: 98px;
    background: #FFF;
    border: 1px solid rgba(189, 189, 189, 0.25);
    box-shadow: 0px 4.71062px 23.5531px rgba(0, 0, 0, 0.07);
    border-radius: 4.71062px;
    padding: 11px 11px 11px 26px;
    direction: flex;
    justify-content: space-between;
  }
  .box .img-bg {
    height: 100%;
    width: 76px;
    border-radius: 5px;
    float: right;
    text-align: center;
  }
  .img-bg img {
    padding-top: 18px;
  }
  .box span {
    color: #BDBDBD;
    text-transform: uppercase;
    font-family: Khula;
    font-style: normal;
    font-weight: 600;
    font-size: 10px;
  }
  .box .c-text {
    font-family: Lato;
    font-style: normal;
    font-weight: normal;
    font-size: 24px;
    color: #2D74DA;
    margin-top: 6px;
  }
  .div-primary {
    background: #1C75BB;
  }
  .div-success {
    background: #17BF5F;
  }
  .div-warning {
    background: #FAD961;
  }
</style>
