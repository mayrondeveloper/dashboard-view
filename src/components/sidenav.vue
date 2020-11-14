<template>
  <div>
    <div class="sidenav" v-bind:class="{ active: menuOpen }">
      <div class="header d-flex">
        <img src="@/assets/image/logo.svg" height="30px" alt="logo">
        <div class="fill-icon menu-item-icon ml-4 d-none" v-on:click="toggleMenu">
          <img src="@/assets/image/icon/list.svg" alt="Menu Icon">
        </div>
      </div>
      <div class="links">
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/home.svg" alt=""></div>
          <div class="nameLink active">Dashboard</div>
          <div class="arrow"><img src="@/assets/image/icon/arrow_bot.svg" alt=""></div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/circle.svg" alt=""></div>
          <div class="nameLink">eCommerce</div>
        </div>
      </div>
      <div class="links">
        <div class="section">
          <div class="title">
            Apps
          </div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/mail.svg" alt=""></div>
          <div class="nameLink boldlink">Email</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/chat.svg" alt=""></div>
          <div class="nameLink boldlink">Chat</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/check-square.svg" alt=""></div>
          <div class="nameLink boldlink">Todo</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/calendar.svg" alt=""></div>
          <div class="nameLink boldlink">Calendar</div>
        </div>
      </div>
      <div class="links">
        <div class="section">
          <div class="title">
            UI ELEMENTS
          </div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/layout.svg" alt=""></div>
          <div class="nameLink boldlink">Grid</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/droplet.svg" alt=""></div>
          <div class="nameLink boldlink">Colors</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/credit-card.svg" alt=""></div>
          <div class="nameLink boldlink">Card</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/grid.svg" alt=""></div>
          <div class="nameLink boldlink">Table</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/archive.svg" alt=""></div>
          <div class="nameLink boldlink">Components</div>
        </div>
      </div>
      <div class="links">
        <div class="section">
          <div class="title">
            FORMS
          </div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/copy.svg" alt=""></div>
          <div class="nameLink boldlink">Form Elements</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/sidebar.svg" alt=""></div>
          <div class="nameLink boldlink">Form Layouts</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/file-text.svg" alt=""></div>
          <div class="nameLink boldlink">From Wizard</div>
        </div>
        <div class="link">
          <div class="icon"><img src="@/assets/image/icon/check-circle.svg" alt=""></div>
          <div class="nameLink boldlink">Form Validation</div>
        </div>
      </div>
    </div>
    <div class="mobile-menu pr-3 d-none" v-show="!isVisible" @click="toggleMenu">
      <div class="fill-icon">
        <img src="@/assets/image/icon/list.svg" alt="Menu icon">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "sidenav",
  data() {
    return {
      menuOpen: false,
      isVisible: false,
    }
  },
  methods: {
    toggleMenu() {
      this.isVisible = !this.isVisible;
      this.menuOpen = !this.menuOpen;
    }
  }
}
</script>

<style scoped lang="scss">

.active {
  margin-left: 0 !important;
  transition: all 0.25s;
  -webkit-transition: all 0.25s;
}

.mobile-menu {
  position: absolute;
  top: 10px;
  z-index: 9;
  left: -5px;
  opacity: 0.5;
  cursor: pointer;
}

@media (max-width: 768px) {
  .sidenav{
    margin-left: -280px;
    position: absolute !important;
    height: auto !important;
  }
  .mobile-menu, .menu-item-icon {
    display: flex !important;
    cursor: pointer;
  }
}

.sidenav {
  min-height: 100vh;
  min-width: 280px;
  position: relative;
  font-family: 'Montserrat', sans-serif;
  width: 280px;
  background: #FAFBFC;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.170509);
  display: flex;
  color: #091e42;
  padding-left: 23px;
  flex-direction: column;
  align-items: flex-start;
  margin-right: 20px;
  z-index: 99;
  height: 100%;

  .header {
    padding-top: 31px;
  }

  .links {
    margin-top: 45px;
    margin-bottom: 20px;
    position: relative;

    .section {
      display: flex;
      padding-left: 13px;

      .title {
        font-family: 'Montserrat', sans-serif;
        color: #FF000A;
        font-size: 14px;
        text-transform: uppercase;
        font-weight: 600;
        justify-content: flex-start;
      }
    }

    .link {
      display: flex;
      flex-direction: row;
      margin-top: 12px;
      position: relative;
      cursor: pointer;

      &:nth-of-type(1) {
        background: #091e42;
        border-radius: 4px;
        padding: 8px 8px 8px 0;
        width: 236px;
      }

      .boldlink {
        font-weight: 500;
      }

      .icon {
        margin-right: 7px;
        margin-left: 13px;
      }

      .nameLink {
        font-family: 'Montserrat', sans-serif;
        color: #172b4d;
        font-size: 15px;
      }

      .nameLink.active {
        color: white;
      }

      .arrow {
        position: absolute;
        top: 6px;
        right: 15px;
      }
    }
  }
}

</style>
