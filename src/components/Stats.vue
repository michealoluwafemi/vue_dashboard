<template>
  <div class="padded">
    <img src="../assets/icons/student-fee.png" />
    <span class="title">General Statistics</span>
    <div>
      <div class="stat-card d-flex" v-for="(stat, key) in statCard"  :key="key">
        <div class="pad">
          <span class="sm">{{ stat.title }}</span>
          <h2>{{ stat.quantity }}</h2>
          <h5 class="c">{{ stat.link }}</h5>
        </div>
        <div class="right">
          <h2 :class="stat.class">{{ stat.stat }}</h2>
          <img :src="stat.imgUrl" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'stats',
  data() {
    return {
      statCard: [
        {
          title: "students",
          quantity: "50, 000",
          link: "view report",
          stat: "+4",
          imgUrl: "",
          class: "success"
        },
        {
          title: "parents",
          quantity: "15, 000",
          link: "view list",
          stat: "+13",
          imgUrl: "",
          class: "success"
        },
        {
          title: "teachers",
          quantity: "5, 000",
          link: "view list",
          stat: "-12",
          imgUrl: "",
          class: "danger"
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
.padded .img {
  margin-top: 10px;
}
.stat-card {
  height: 89.49px;
  background: #FFFFFF;
  border: 1px solid rgba(189, 189, 189, 0.25);
  box-sizing: border-box;
  box-shadow: 0px 4.71062px 23.5531px rgba(0, 0, 0, 0.07);
  border-radius: 4.71062px;
  margin-top: 10px;
}
.stat-card .sm {
  font-family: Khula;
  font-style: normal;
  font-weight: 600;
  font-size: 10px;
  text-transform: uppercase;
  color: #BDBDBD;
}
.stat-card h2 {
  font-family: Khula;
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  color: #3B3B3B;
}
.stat-card .c {
  font-family: Khula;
  font-style: normal;
  font-weight: bold;
  font-size: 10px;
  text-transform: uppercase;
  color: #1B75BB;
}
.stat-card .pad {
  margin-left: 26px;
  margin-top: 8px;
  width: 100px;
}
.right {
  width: 90px;
  text-align: center;
}
.right h2 {
  font-family: Khula;
  font-style: normal;
  font-weight: 300;
  font-size: 24.6969px;
  color: #17BF5F;
}
.danger {
  color: #FB5D5D;
}
.success {
  color: #17BF5F;
}
</style>
