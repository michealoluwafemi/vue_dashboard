<template>
  <aside class="app-sidebar">
    <div class="logo-brand">
      <img alt="App Logo" src="../assets/images/logo.png">
      <span>Handmaid's International</span>
    </div>
    <ul class="nav-links">
      <li class="link" v-for="(link, key) in links" :key="key">
        <i :class="link.icon"></i>{{ link.title.charAt(0).toUpperCase() + link.title.slice(1) }}
      </li>
    </ul>
  </aside>
</template>

<script>
import '../assets/fonts/css/all.css'
export default {
  name: 'Sidebar',
  props: {

  },
  data() {
    return {
      links: [
        {
          icon: "fa fa-dashboard",
          title: "dashboard"
        },
        {
          icon: "fa fa-graduation-cap",
          title: "students"
        },
        {
          icon: "fa fa-dashboard",
          title: "employees"
        },
        {
          icon: "fa fa-users",
          title: "guardians"
        },
        {
          icon: "fa fa-dashboard",
          title: "attendance"
        },
        {
          icon: "fa fa-users",
          title: "finance"
        },
        {
          icon: "fa fa-dashboard",
          title: "subjects"
        },
        {
          icon: "fa fa-users",
          title: "batches"
        },
        {
          icon: "fa fa-dashboard",
          title: "report cards"
        },
        {
          icon: "fa fa-users",
          title: "SMS"
        },
        {
          icon: "fa fa-calendar",
          title: "events"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo-brand {
  background: #FFF;color: #3B3B3B;
  height: 70px;
  text-align: center;
}
.app-sidebar {
  background: linear-gradient(136.25deg, #1B75BB 0%, #00ADEE 100%);
  height: 100%;
  color: #ffffff;
  width: 265px;
}
.nav-links {
  padding: 3em 2em;
  list-style: none;
  margin: 0;
}
.link {
  padding: 0.5em 1em;
  margin-bottom: 0.5em;
}.link i {margin-right: 16px;}
.link:hover {
  cursor: pointer;
  background: #ffffff;
  color: rgb(0, 28, 184);
  border-radius: 4px;
}
</style>
