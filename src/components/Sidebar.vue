<template>
  <aside class="app-sidebar">
    <div class="logo-brand">
      <img alt="App Logo" src="../assets/images/logo.png">
      <span>Handmaid's International</span>
    </div>
    <ul class="nav-links">
      <li class="link">
        <router-link
          to="/"
        ><img src="../assets/icons/dashboard.png" />Dashboard
        </router-link>
      </li>
      <li class="link dropdown-toggle" data-toggle="dropdown">
        <router-link
          to=""
          ><img src="../assets/icons/student.png" />Students
        </router-link>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Class 1</a></li>
          <li><a class="dropdown-item" href="#">Class 1</a></li>
        </ul>
      </li>
      <li class="link dropdown-toggle" data-toggle="dropdown">
        <router-link
          to=""
        ><img src="../assets/icons/employer.png" />Employees
        </router-link>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Employees 1</a></li>
        </ul>
      </li>
      <li class="link">
        <router-link
          to=""
        ><img src="../assets/icons/guardian.png" />Guardians
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink">
        <router-link
          to=""
        ><img src="../assets/icons/attendance.png" />Attendance
        </router-link>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Attendance 1</a></li>
        </ul>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink">
        <router-link
          to=""
        ><img src="../assets/icons/finance.png" />Finance
        </router-link>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Finance 1</a></li>
        </ul>
      </li>
      <li class="link">
        <router-link
          to=""
        ><img src="../assets/icons/subject.png" />Subjects
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        ><img src="../assets/icons/batches.png" />Batches
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        ><img src="../assets/icons/report.png" />Report Cards
        </router-link>
      </li>
      <li class="link">
        <router-link
          to=""
        ><img src="../assets/icons/sms.png" />SMS
        </router-link>
      </li>
      <li class="link dropdown-toggle" id="dropdownMenuLink">
        <router-link
          to=""
        ><img src="../assets/icons/events.png" />Events
        </router-link>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item" href="#">Event 1</a></li>
        </ul>
      </li>
      <!-- <li class="link" v-for="(link, key) in links" :key="key">
        <router-link
          :to="link.to"
          >
          {{ link.title.charAt(0).toUpperCase() + link.title.slice(1) }}
        </router-link>
      </li> -->
      <hr class="hr" />
      <li class="link">
        <route-link
          to=""
        >Settings
        </route-link>
      </li>
    </ul>

    <ul class="horizontal">
      <li class="wrap">Help</li>
      <li>Terms.Privacy</li>
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
.horizontal {
  display: inline-flex;
}
.horizontal li {
  list-style: none;
  height: 30px;
}
li img {
  margin-right: 20px;
  width: 18px;
  height: 18px;
}
.horizontal .wrap {
  font-family: Khula;
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  text-align: center;
  background: #FFF;
  color: #1C75BB;
  padding: 5px 14px 5px 14px;
  border-radius: 17px;
  margin-right: 15px;
}
.hr {
  background: #FFF;
  height: 0.2px;
}
.dropdown {
  margin-left: 76px !important;
}
.logo-brand {
  background: #FFF;color: #3B3B3B;
  height: 70px;
  padding-top: 17px;
}
.dropdown-menu {
  background: linear-gradient(136.25deg, #1B75BB 0%, #00ADEE 100%);
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
  font-family: Khula;
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
}
.link:hover, .dropdown-item:hover {
  cursor: pointer;
  background: #1C75BB;
  border-radius: 4px;
}
</style>
