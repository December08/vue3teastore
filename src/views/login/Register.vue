<template>
  <div class="register">
    <div class="register__wrapper">
      <div class="register__account">
        <div class="register__title">请输入手机号：</div>
        <div class="register__content">
          <span class="iconfont register__content-img" >&#xe62a;</span>
          <input type="text" class="register__account-input">
        </div>
      </div>
      <div class="register__password">
        <div class="register__title">请输入密码：</div>
        <div class="register__content">
          <span class="iconfont register__content-img">&#xe620;</span>
          <input type="password" class="register__password-input">
        </div>
      </div>
      <div class="register__password">
        <div class="register__title">请再次输入密码：</div>
        <div class="register__content">
          <span class="iconfont register__content-img">&#xe620;</span>
          <input type="password" class="register__password-input">
        </div>
      </div>
      <div class="register__button">注册</div>
    </div>
  </div>
</template>

<script >

export default {
  name: 'register',
  setup () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.register {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  border-radius: 20px;
  background: white;
  &__wrapper {
    position: relative;
    padding: .3rem .16rem;
  }
  &__account {
    flex: 1;
    &-input {
      flex: 1;
      margin: 0 .12rem;
      font-size: .16rem;
      width: 100%;
      height: 100%;
      border-color: none;
      border: none;
      outline: none;
      background-color: transparent;
      color: #343434;
    }
  }
  &__password {
    flex: 1;
    margin-top: .27rem;
    &-input {
      margin: 0 .12rem;
      font-size: .16rem;
      width: 100%;
      height: 100%;
      border-color: none;
      border: none;
      outline: none;
      background-color: transparent;
      color: #343434;
    }
  }
  &__title {
    font-size: .16rem;
    color: #c57b53;
  }
  &__content {
    width: 100%;
    border-radius: 44px;
    height: .44rem;
    margin-top: .11rem;
    background: #DBC5B9;
    display: flex;
    align-items: center;
    &-img {
      margin-left: .2rem;
      color: #fff;
      font-size: .16rem;
    }
  }
  &__button {
    flex: 1;
    margin: .36rem 0 .2rem 0;
    height: .44rem;
    background-color: #c99274;
    border-radius: .44rem;
    font-size: .16rem;
    text-align: center;
    line-height: .44rem;
    color: #fff;
  }
}
</style>
