<template>
  <div class="l-navbar" id="nav-bar" :class="{ show: sidebarStatus }">
    <nav class="nav">
      <div class="div-logo text-center">
        <img
          v-show="sidebarStatus"
          id="logo"
          src="../assets/logo.png"
          alt="Save the future logo"
        />
      </div>
      <div class="main-nav-div">
        <a href="#" class="nav_link active"
          ><box-icon color="white" name="planet"></box-icon>
          <span class="nav_name"> SaveTheFuture</span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" name="shopping-bag" type="solid"></box-icon>
          <span locked="false" class="nav_name">Shop </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" type="solid" name="user-badge"></box-icon>
          <span locked="true" class="nav_name"
            >Teams &amp; Profile
            <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" name="category"></box-icon>
          <span locked="true" class="nav_name"
            >Marketplace <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" type="solid" name="diamond"></box-icon>
          <span locked="true" class="nav_name"
            >Collectibles <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" name="coin-stack"></box-icon>
          <span locked="true" class="nav_name"
            >Lottery <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" name="binoculars" type="solid"></box-icon>
          <span locked="true" class="nav_name"
            >Predict the future
            <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <a href="#" class="nav_link">
          <box-icon color="white" name="plus"></box-icon>
          <span locked="true" class="nav_name"
            >More <box-icon color="white" name="lock-alt"></box-icon>
          </span>
        </a>
        <div v-show="sidebarStatus" class="sub-nav-div">
          <p>
            <img
              id="social-logo"
              src="../assets/twitter-logo.png"
              alt="Twitter logo"
            />
            <img
              id="social-logo"
              src="../assets/discord-logo.png"
              alt="Discord logo"
            />
          </p>
          <p><span class="accent">1 $TF</span> = $ 0.00000000384</p>
          <p>&copy; Save The Future</p>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "TheSidebar",
  props: {
    sidebarStatus: Boolean,
  },
};
</script>

<style scoped></style>
