<template>
  <div class="d-flex flex-row justify-content-lg-between mt-n2">
    <div class="input-group d-flex">
      <b-form-input placeholder="Search hear"></b-form-input><img class="search-icon" src="@/assets/image/icon/search.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "searchInput"
}
</script>

<style scoped lang="scss">
.input-group {
  width: 100%;
  background: #FFFFFF;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  border: none;
  height: 62px;
  input {
    border: none;
    height: 62px;
    &::placeholder {
      font-size: 22px !important;
      font-weight: 300;
    }
  }
}
.search-icon {
  position: absolute;
  right: 33px;
  top: 20px;
}

</style>
