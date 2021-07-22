<template>
  <header class="header" :class="{ 'header-show': sidebarStatus }" id="header">
    <div @click="$emit('toggleSidebar')" class="header-toggle">
      <box-icon name="menu" id="header-toggle"></box-icon>
    </div>
    <div>
      <button type="button" class="btn btn-primary btn-header">
        Connect
      </button>
      <img class="icon-user" src="../assets/icon-user.png" alt="User icon" />
    </div></header
></template>

<script>
export default {
  name: "TheNavbar",
  props: {
    sidebarStatus: Boolean,
  },
};
</script>

<style scoped></style>
