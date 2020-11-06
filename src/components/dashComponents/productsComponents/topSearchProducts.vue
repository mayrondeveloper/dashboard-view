<template>
  <div>
    <div class="d-flex flex-row justify-content-lg-between row no-gutters">
      <div class="col-md-6 col-sm-12">
        <div class="top-title">7,618 results found in 5ms</div>
      </div>
      <div class="col-md-6 col-sm-12 mt-sm-5 mt-md-0">
        <div class="d-flex flex-row align-items-center icons-top justify-content-md-end justify-content-sm-start">
          <div>
            <b-dropdown id="dropdown-1" text="Default" style="height: 40px; padding-right: 10px;"
                        class="m-md-2 dropdownPrimary-ma">
              <b-dropdown-item>First Action</b-dropdown-item>
              <b-dropdown-item>Second Action</b-dropdown-item>
              <b-dropdown-item>Third Action</b-dropdown-item>
            </b-dropdown>
          </div>
          <div class="fill-icon mr-3"><img src="@/assets/image/icon/grid.svg" alt=""></div>
          <div class="fill-icon"><img src="@/assets/image/icon/list.svg" alt=""></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "topSearchProducts"
}
</script>

<style scoped>
.icons-top {
  align-items: center;
  position: relative;
  top: -29px;
  justify-content: end;
}
</style>
