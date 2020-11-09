<template>
  <div class="row topbar-desk mt-4 topbar no-gutters">
    <div class="col-md-6 left-elements d-flex justify-content-start">
      <ul class="ul-left-elements">
        <li><img src="@/assets/image/icon/check-square.svg" alt=""></li>
        <li><img src="@/assets/image/icon/chat.svg" alt=""></li>
        <li><img src="@/assets/image/icon/mail.svg" alt=""></li>
        <li><img src="@/assets/image/icon/calendar.svg" alt=""></li>
        <li><img src="@/assets/image/icon/star.svg" alt=""></li>
      </ul>
    </div>
    <div class="col-md-6 right-elements d-flex justify-content-end">
      <ul class="ul-right-elements">
        <li>
          <div class="language">English</div>
        </li>
        <li><img src="@/assets/image/icon/bell.svg" alt=""></li>
        <li><img src="@/assets/image/icon/search.svg" alt=""></li>
        <li>
          <div class="avatar d-flex flex-row">
            <div class="id d-flex flex-column">
              <div class="name">John Doe</div>
              <span class="status">Avaiable</span>
            </div>
            <div>
              <img src="@/assets/image/icon/Oval.svg" alt="">
            </div>
          </div>
        </li>

      </ul>
    </div>
    <div class="mobile-icon pr-3 d-none">
        <img src="@/assets/image/icon/Oval.svg" alt="" @click="visibleMobile">
    </div>

    <div v-if="isVisible" class="card-ma mobile-card d-flex flex-column-reverse justify-content-center align-items-end">
      <div class="sample">
        <div>
          <div class="language">English</div>
        </div>
        <div class="d-flex flex-row mt-2">
          <div class="mr-3"><img src="@/assets/image/icon/bell.svg" alt=""></div>
          <div><img src="@/assets/image/icon/search.svg" alt=""></div>
        </div>
        <div class="">
          <div class="avatar d-flex flex-row">
            <div class="id d-flex flex-column mt-2">
              <div class="name">John Doe</div>
              <span class="status">Avaiable</span>
            </div>
<!--            <div>-->
<!--              <img src="@/assets/image/icon/Oval.svg" alt="">-->
<!--            </div>-->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "topbar",
  data() {
    return {
      isVisible: false
    }
  },
  methods: {
    visibleMobile() {
      this.isVisible = !this.isVisible;
    }
  }
}
</script>

<style scoped lang="scss">
@media (max-width: 990px) {
  .mobile-icon {
    display: flex !important;
  }
  .right-elements {
   display: none !important;
  }
}

.mobile-icon {
  cursor: pointer;
  position: absolute;
  right: 20px;
  top: 37px;
}

.mobile-card {
  z-index: 2;
  position: absolute;
  right: 11px;
  top: 79px;

  .sample {
    position: relative;
    &:before {
      content: "";
      display: inline-block;
      vertical-align: middle;
      margin-right: 10px;
      width: 0;
      height: 0;
      position: absolute;
      top: -25px;
      right: 10px;
      border-left: 10px solid transparent;
      border-right: 10px solid transparent;
      border-bottom: 10px solid white;
    }
  }
}

ol {
  list-style: none;
}

ul {
  display: flex;
  flex-direction: row;
  list-style: none;
}

.topbar {
  height: 68px;
  background: #FFFFFF;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #36B37E;
  ul {
    display: flex;
    flex-direction: row;
    list-style: none;
    padding: 0 20px;
    margin: 0;
    align-items: center;

    li {
      padding: 0 5px;
    }
  }

  .left-elements {
    li {
      margin-right: 10px;
      cursor: pointer;
    }
  }

  .right-elements {
    li {
      margin-left: 21px;
      cursor: pointer;
    }
  }

  .avatar {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    color: #0052cc;
    font-weight: 500;
    .id {
      display: flex;
      flex-direction: column;
      align-items: end;
      margin-right: 10px;

      .name {
        font-size: 14px;
      }

      .status {
        font-size: 11px;
        font-weight: 300;
      }
    }
  }
}
</style>
