<template>
  <div class="padded">
    <img src="../assets/icons/student-fee.png" />
    <span class="title">Student Fees</span>
    <div class="img">
      <img src="../assets/images/performance.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Perf',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.padded {
  margin-top: 30px;
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
</style>
