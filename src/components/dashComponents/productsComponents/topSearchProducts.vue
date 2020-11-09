<template>
  <div>
    <div class="d-flex flex-row justify-content-lg-between row no-gutters">
      <div class="col-md-6 col-12">
        <div class="top-title">7,618 results found in 5ms</div>
      </div>
      <div class="col-md-6 col-12 mt-md-0">
        <div
          class="d-flex flex-row align-items-center icons-top justify-content-md-end justify-content-start pt-5 pt-md-0">
          <div class="mr-2 filter-button">
            <button class="filterButton" v-on:click="modal">Filters</button>
          </div>
          <div>
            <b-dropdown id="dropdown-1" text="Default" style="padding-right: 10px; color: #36B37E;"
                        class="m-md-2 dropdownPrimary-ma dropdown-ma-arrow d-flex text-left">
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
  name: "topSearchProducts",
  methods: {
    modal() {
      this.$bvModal.show('modal-1')
    }
  }
}
</script>

<style lang="scss">
.icons-top {
  align-items: center;
  position: relative;
  top: -29px;
  justify-content: end;
}

.filter-button {
  display: none;
}

.dropdown-ma-arrow {
  button {
    background: #36b37e;
    color: #36B37E;
  }
  &:hover {
    color: #36B37E;
  }
  &:active {
    color: #36B37E;
  }
  &:focus, &:focus-visible, &:focus-within {
    color: #36B37E;
  }
}

.dropdown-toggle::after {
  border: none !important;
}

@media (max-width: 1500px) {
  .filter-button {
    display: flex !important;
  }
}
</style>
