<template>
  <aside class="app-sidebar">
    <div class="logo-brand">
      <img alt="App Logo" src="../assets/images/logo.png">
      <span>Handmaid's International</span>
    </div>
    <ul class="nav-links">
      <li class="link">
        <router-link
          to=""
        >Dashboard
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link
          to=""
          >Students
        </router-link>
        <ul class="dropdown-menu" aria-labelledby="dropdownMenuLink">
          <li><a class="dropdown-item" href="#">Class 1</a></li>
        </ul>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link
          to=""
        >Employees
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        >Guardians
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link
          to=""
        >Attendance
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link
          to=""
        >Finance
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        >Subjects
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        >Batches
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        >Report Cards
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        >SMS
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link
          to=""
        >Events
        </router-link>
      </li>
      <!-- <li class="link" v-for="(link, key) in links" :key="key">
        <router-link
          :to="link.to"
          >
          {{ link.title.charAt(0).toUpperCase() + link.title.slice(1) }}
        </router-link>
      </li> -->
    </ul>
  </aside>
</template>

<script>
export default {
  name: 'Sidebar',
  props: {

  },
  data() {
    return {
      links: [
        {
          icon: "../assets/images/dashboard.png",
          to: "/",
          title: "dashboard"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.dropdown {
  margin-left: 76px !important;
}
.logo-brand {
  background: #FFF;color: #3B3B3B;
  height: 70px;
  padding-top: 17px;
}
.app-sidebar {
  background: linear-gradient(136.25deg, #1B75BB 0%, #00ADEE 100%);
  height: 100%;
  color: #ffffff;
  width: 276px;
}
.nav-links {
  padding: 3em 2em;
  list-style: none;
  margin: 0;
}
.link {
  padding: 0.5em 1em;
  margin-bottom: 0.5em;
}
.link i {
  margin-right: 16px;
}
.link a {
  color: #FFF !important;
  text-decoration: none;
}
.link:hover {
  cursor: pointer;
  background: #1C75BB;
  border-radius: 4px;
}
</style>
