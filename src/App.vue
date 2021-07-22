<template>
  <div id="app">
    <TheNavbar
      :sidebarStatus="isSidebar"
      @toggleSidebar="isSidebar = !isSidebar"
    />
    <TheSidebar :sidebarStatus="isSidebar" />
    <Home />
  </div>
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";
import TheSidebar from "./components/TheSidebar.vue";
import Home from "./components/Home.vue";

export default {
  name: "App",
  components: {
    TheNavbar,
    TheSidebar,
    Home,
  },

  data() {
    return {
      isSidebar: true,
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Kanit:wght@400;700&display=swap");

/* Vars */
:root {
  --header-height: 3rem;
  --nav-width: 68px;
  --first-color: #132832;
  --secondary-color: #8d8d8d;
  --first-color-light: #ddd;
  --light-color: #e4f5f2;
  --accent-color: #65debb;
  --accent-secondary-color: #cc85d5;
  --background-color: #060809;
  --transparent-box: rgba(49, 97, 120, 0.4);
  --z-fixed: 100;
}

/* Images/Icons */
.nav_name box-icon {
  width: 14px;
  opacity: 0.4;
}
.header box-icon {
  width: 50px;
}
.div-bottom .btn box-icon {
  width: 14px;
}
#logo {
  width: 120px;
}
#social-logo {
  width: 20px;
  margin-right: 10px;
}
.icon-small {
  width: 30px;
}
.icon-user {
  width: 40px;
}
.table-cell .icon-small {
  margin: 10px 0;
}
.icon {
  width: 50px;
}

/* Layout/Elements */
body {
  background-image: url("./assets/fern-bg.jpeg");
  background-color: var(--background-color) !important;
}
.header {
  width: 100%;
  height: var(--header-height);
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 1rem;
  background-color: var(--light-color);
  z-index: var(--z-fixed);
  transition: 0.5s;
}

.table {
  display: table;
}
.table-cell {
  display: table-cell;
  vertical-align: top;
  line-height: 0.8em;
}
.table-cell h3 {
  margin-top: 4px;
}

.header-toggle {
  color: var(--first-color);
  font-size: 1.5rem;
  cursor: pointer;
}

/* Buttons */
.btn {
  color: #fff !important;
  border-radius: 100px !important;
  border: 0 !important;
}
.btn-primary {
  background-color: var(--first-color) !important;
}
.btn-header {
  width: 160px;
  margin-right: 20px;
}
.btn-accent-secondary {
  background-color: var(--accent-secondary-color) !important;
}
.btn-accent {
  background-color: var(--accent-color) !important;
}
.btn-secondary {
  background-color: var(--secondary-color) !important;
}

/* Navbar */
.header-img {
  width: 35px;
  height: 35px;
  display: flex;
  justify-content: center;
  border-radius: 50%;
  overflow: hidden;
}
.header-img img {
  width: 40px;
}

/* Sidebar */
.l-navbar {
  position: fixed;
  top: 0;
  left: -30%;
  width: var(--nav-width);
  height: 100vh;
  background-color: var(--first-color);
  padding: 0.5rem 1rem 0 0;
  transition: 0.5s;
  z-index: var(--z-fixed);
}
.nav {
  height: 100%;
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

/* Home */
.main-div {
  text-align: center;
  margin-top: 100px;
}
.main-div .row {
  padding: 0 200px 0 300px;
}
.div-bottom {
  position: absolute;
  bottom: 10px;
  width: 100%;

  padding-right: 36px;
}
.column {
  border-radius: 20px;
  height: 200px;
  padding: 20px;
  position: relative;
}
#col-first {
  background-color: var(--light-color);
}
#col-second {
  background-color: var(--transparent-box);
  color: #fff;
}
#col-third,
#col-fifth,
#col-sixth,
#col-seventh {
  background-color: var(--transparent-box);
  color: #fff;
}
#col-fourth {
  background-color: #dee2f6;
}
#col-fourth h5 {
  margin-top: 46px;
}
.center p {
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
#col-sixth,
#col-seventh {
  background-color: rgba(0, 0, 0, 0.5);
  box-shadow: 0 0 5px 2.5px rgba(96, 60, 60, 0.2),
    0 0 8px 5px rgba(17, 255, 0, 0.2), 0 0 11.5px 7.5px rgba(0, 255, 255, 0.2);
  color: #fff;
}
#col-sixth p {
  color: #fff;
}
#col-seventh div {
  margin-top: 30px;
  line-height: 0.8em;
  font-size: 0.8em;
}

.main-nav-div {
  margin-top: 38px;
  font-size: 0.9em;
}
.sub-nav-div {
  position: absolute;
  padding: 0.5rem 0 0.5rem 1.5rem;
  bottom: 0px;

  line-height: 1;

  font-size: 0.7em;
}
.sub-nav-div hr {
  margin: 0.3rem;
  color: #fff;
}
.sub-nav-div p {
  color: #fff;
}

.nav_logo,
.nav_link {
  display: grid;
  grid-template-columns: max-content max-content;
  align-items: center;
  column-gap: 1rem;
  padding: 0.5rem 0 0.5rem 1.5rem;
}
.nav_logo {
  margin-bottom: 2rem;
}
.nav_logo-icon {
  font-size: 1.25rem;
  color: var(--light-color);
}
.nav_logo-name {
  color: var(--light-color);
  font-weight: 700;
}
.nav_link {
  position: relative;
  color: var(--first-color-light);
  margin-bottom: 1rem;
  transition: 0.3s;
}
.nav_link:hover {
  color: var(--light-color);
}

.show {
  left: 0;
}
.body-pd {
  padding-left: calc(var(--nav-width) + 1rem);
}

/* Typography */
* {
  font-family: "Kanit";
}
a {
  text-decoration: none !important;
  color: var(--secondary-color) !important;
  transition: all 0.25s;
}
[locked="false"]:hover {
  color: #fff !important;
  transition: all 0.25s;
}
.active {
  color: var(--accent-color) !important;
}
.gray {
  color: var(--secondary-color);
}
.bolder {
  font-weight: bolder;
}
.accent {
  color: var(--accent-color);
}
.accent-secondary {
  color: var(--accent-secondary-color);
}

/* Responsiveness */
@media screen and (max-width: 800px) {
  .main-div .row {
    padding: 10px 20px;
    margin-left: 60px;
  }

  #logo,
  .sub-nav-div {
    display: none;
  }
}
@media screen and (max-width: 1000px) {
  .main-div .row {
    padding: 10px 40px;
    margin-left: 80px;
  }
}
@media screen and (min-width: 1200px) {
  .main-div .row {
    padding: 10px 190px;
    margin-left: 80px;
  }
}
@media screen and (min-width: 768px) {
  body {
    margin: calc(var(--header-height) + 1rem) 0 0 0;
    padding-left: calc(var(--nav-width) + 2rem);
  }
  .header {
    height: calc(var(--header-height) + 1rem);
    padding: 0 2rem 0 calc(var(--nav-width) + 1.5rem);
  }
  .header-show {
    padding-left: calc(var(--nav-width) + 1.5rem + 156px);
  }

  .header-img {
    width: 40px;
    height: 40px;
  }

  .header-img img {
    width: 45px;
  }

  .l-navbar {
    left: 0;
    padding: 1rem 1rem 0 0;
  }

  .show {
    width: calc(var(--nav-width) + 156px);
  }

  .body-pd {
    padding-left: calc(var(--nav-width) + 188px);
  }
}
</style>
