<template>
  <div class="main-div">
    <div class="row">
      <div class="col-sm-12 col-md-6 col-lg-6">
        <div class="column" id="col-first">
          <h3 class="bolder">
            <span class="">100.000</span> <span class="accent">$TF</span>
          </h3>
          <p class="small">Your $TF balance</p>
          <div class="d-grid gap-2 div-bottom">
            <button class="btn btn-accent" type="button">Buy</button>
            <button class="btn btn-primary" type="button">
              Unlock wallet
            </button>
          </div>
        </div>
      </div>
      <div class="col-sm-12 col-md-6 col-lg-6">
        <div class="column" id="col-second">
          <img
            class="icon-small"
            src="../assets/icon-lock.png"
            alt="NFTs logo"
          />
          <div class="d-grid gap-2 div-bottom">
            <p class="small gray">Your green NFTs</p>
            <button class="btn btn-secondary" type="button">Farm</button>
            <button class="btn btn-secondary" type="button">
              Unlock wallet
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12 col-md-3 col-lg-3">
        <div class="column" id="col-third">
          <p class="small">Referral</p>
          <img class="icon" src="../assets/icon-ref.png" alt="Referral logo" />
          <div class="d-grid gap-2 div-bottom">
            <button class="btn btn-secondary" type="button">
              Your referrals
            </button>
          </div>
        </div>
      </div>
      <div class="col-sm-12 col-md-6 col-lg-6">
        <div class="column" id="col-fourth">
          <h5 class="bolder">Get your cool eco-products</h5>
          <div class="d-grid gap-2 div-bottom">
            <button class="btn btn-accent-secondary" type="button">
              Redeem
            </button>
          </div>
        </div>
      </div>
      <div class="col-sm-12 col-md-3 col-lg-3">
        <div class="column" id="col-fifth">
          <p class="small">Ranking</p>
          <img class="icon" src="../assets/icon-trophy.png" alt="Ranking logo" />
          <div class="d-grid gap-2 div-bottom">
            <button class="btn btn-secondary" type="button">
              Your ranking
            </button>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-sm-12 col-md-6 col-lg-6">
        <div id="col-sixth" class="column">
          <h5>Statistics</h5>
          <div class="table">
            <div class="table-cell">
              <img
                class="icon-small"
                src="../assets/icon-holders.png"
                alt="Ranking logo"
              />
              <h3 class="accent-secondary">17.500</h3>
              <p class="small">Holders</p>
            </div>
            <div class="table-cell">
              <img
                class="icon-small"
                src="../assets/icon-burn.png"
                alt="Ranking logo"
              />
              <h3 class="accent-secondary">458</h3>
              <p class="small">Burned coins</p>
            </div>
            <div class="table-cell">
              <img
                class="icon-small"
                src="../assets/icon-market-cap.png"
                alt="Ranking logo"
              />
              <h3 class="accent-secondary">248k</h3>
              <p class="small">Market cap</p>
            </div>
          </div>
        </div>
      </div>
      <div class="col-sm-12 col-md-6 col-lg-6">
        <div id="col-seventh" class="column">
          <h5>Available soon</h5>
          <div>
            <p>May, 2021 &mdash; Referral + ranking</p>
            <p>June, 2021 &mdash; <span class="accent">Green NFTs</span></p>
            <p>
              Sept., 2021 &mdash;
              <span class="accent-secondary">Products</span>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div></template
>

<script>
export default {
  name: "TheNavbar",
  // props: {},
};
</script>

<style scoped></style>
