<template>
  <div class="padded">
    <img src="../assets/icons/student-fee.png" />
    <span class="title">Absent Students</span>
    <div class="absent">

    </div>
  </div>
</template>

<script>
export default {
  name: 'absent',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.absent {
  background: #FFF;
  width: 259px;
  height: 233px;
  border: 1px solid rgba(189, 189, 189, 0.25);
  box-sizing: border-box;
  box-shadow: 0px 7.51481px 37.574px rgba(0, 0, 0, 0.07);
  border-radius: 7.51481px;
}
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
</style>
