<template>
  <div class="row d-flex pt-4 mb-5 no-gutters pl-1" style="margin-left: -6px;">
    <div class="col-md-11 d-flex justify-content-start align-items-center flex-row columns">
      <div class="component">Card Actions</div>
      <img src="@/assets/image/icon/pipe.svg" height="32" alt="">
      <img src="@/assets/image/icon/home.svg" height="18" alt="">
      <img src="@/assets/image/icon/chevrons-right.svg" height="10" alt="">
      <div class="breadcrumb-item">eCommerce</div>
      <img src="@/assets/image/icon/chevrons-right.svg" height="10" alt="">
      <div class="breadcrumb-item">Eletronics</div>
    </div>
    <div class="col-md-1 d-flex pt-2 pt-md-0 justify-content-start justify-content-md-end">
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
  @media (max-width: 768px) {
    font-size: 15px;
  }
  @media (max-width: 374px) {
    padding-right: 5px !important;
    margin: 0;
    font-size: 13px;
  }
}

.breadcrumb-item {
  font-size: 14px;
  @media (max-width: 768px) {
    font-size: 12px;
  }
}

.columns > img, .columns > div {
  padding-right: 14px;
  @media (max-width: 374px) {
    padding-right: 4px;
  }
}

</style>
