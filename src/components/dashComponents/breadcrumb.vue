<template>
  <div class="row d-flex pt-4 mb-5 no-gutters pl-1" style="margin-left: -6px;">
    <div class="col-md-6 d-flex justify-content-start align-items-center flex-row columns">
      <div class="component ">Card Actions</div>
      <img src="@/assets/image/icon/pipe.svg" alt="">
      <img src="@/assets/image/icon/home.svg" alt="">
      <img src="@/assets/image/icon/chevrons-right.svg" alt="">
      <div class="breadcrumb-item">eCommerce</div>
      <img src="@/assets/image/icon/chevrons-right.svg" alt="">
      <div class="breadcrumb-item">Eletronics</div>
    </div>
    <div class="col-md-6 d-flex justify-content-end">
      <div class="circle">
        <img src="@/assets/image/icon/settings.svg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "breadcrumb"
}
</script>

<style scoped lang="scss">
.circle {
  width: 40px;
  height: 40px;
  background-color: #686868;
  border-radius: 20px;
  display: flex;
  cursor: pointer;

  img {
    margin: 0 auto;
  }
}

.component {
  font-size: 24px;
}

.breadcrumb-item {
  font-size: 14px;
}

.columns > img, .columns > div {
  padding-right: 14px;
}

</style>
