<template>
  <div class="sidenav">
    <div class="header">
      <img src="@/assets/image/logo.svg" height="30px" alt="logo">
    </div>
    <div class="links">
      <div class="link">
        <div class="icon"><img src="@/assets/image/icon/home.svg" alt=""></div>
        <div class="nameLink">Dashboard</div>
        <div class="arrow"><img src="@/assets/image/icon/arrow_bot.svg" alt=""></div>
      </div>
      <div class="link">
        <div class="icon"><img src="@/assets/image/icon/circle.png" alt=""></div>
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
</template>

<script>
export default {
name: "sidenav"
}
</script>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
  .sidenav {
    @media (max-width: 768px) {
      display: none;
    }
    min-height: 100vh;
    min-width: 280px;
    position: relative;
    font-family: 'Montserrat', sans-serif;
    width: 280px;
    background: #FFFFFF;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.170509);
    display: flex;
    color: #cecece;
    height: auto;
    padding-left: 23px;
    flex-direction: column;
    align-items: flex-start;
    margin-right: 20px;
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
          color: #999999;
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
        &:nth-of-type(1) {
          background: #ECECEC;
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
          color: #2C2C2C;
          font-size: 15px;
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
