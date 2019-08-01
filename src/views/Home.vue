<template>
  <div class="home">
    <StuFees />
    <div class="stats">
      <Stats />
    </div>
    <div class="perf">
      <Perf />
    </div>
    <div>
      <div class="recentTransactions">
        <RecentTransactions />
      </div>
      <div class="absent">
        <Absent />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import StuFees from '@/components/StuFees.vue'
import Perf from '@/components/Perf.vue'
import Stats from '@/components/Stats.vue'
import Absent from '@/components/Absent.vue'
import RecentTransactions from '@/components/RecentTransactions.vue'

export default {
  name: 'home',
  components: {
    StuFees,
    Perf,
    Stats,
    Absent,
    RecentTransactions
  }
}
</script>

<style scoped>
.stats {
  width: 280px;
  margin-left: 20px;
  float: right;
}
.perf {
}
.absent {
  float: left;
}
</style>
