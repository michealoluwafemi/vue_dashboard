<template>
  <div class="padded">
    <div class="table-card">
    </div>
    <img src="../assets/icons/student-fee.png" />
    <span class="title">Recent Transactions</span>
  </div>
</template>

<script>
export default {
  name: 'recentTransactions',
  data() {
    return {

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
.padded .img {
  margin-top: 10px;
}
.table-card {
  background: #FFFFFF;
  border: 1px solid rgba(189, 189, 189, 0.25);
  box-sizing: border-box;
  box-shadow: 0px 4.71062px 23.5531px rgba(0, 0, 0, 0.07);
  border-radius: 4.71062px;
  margin-top: 10px;
}
</style>
