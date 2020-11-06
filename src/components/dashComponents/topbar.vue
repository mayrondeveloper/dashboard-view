<template>
  <div class="row mt-4 topbar no-gutters">
    <div class="col-md-6 left-elements d-flex justify-content-start">
      <ul>
        <li><img src="@/assets/image/icon/check-square.svg" alt=""></li>
        <li><img src="@/assets/image/icon/chat.svg" alt=""></li>
        <li><img src="@/assets/image/icon/mail.svg" alt=""></li>
        <li><img src="@/assets/image/icon/calendar.svg" alt=""></li>
        <li><img src="@/assets/image/icon/star.svg" alt=""></li>
      </ul>
    </div>
    <div class="col-md-6 right-elements d-flex justify-content-end">
      <ul>
        <li><div class="language">English</div></li>
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
  </div>
</template>

<script>
export default {
  name: "topbar"
}
</script>

<style scoped lang="scss">
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
