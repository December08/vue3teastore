<template>
  <div class="login">
    <div class="login__wrapper">
      <div class="login__account">
        <div class="login__title">账号</div>
        <div class="login__content">
          <span class="iconfont login__content-img" >&#xe62a;</span>
          <input type="text" class="login__account-input">
        </div>
      </div>
      <div class="login__password">
        <div class="login__title">密码</div>
        <div class="login__content">
          <span class="iconfont login__content-img">&#xe620;</span>
          <input type="password" class="login__password-input">
        </div>
      </div>
      <div class="login__button">登录</div>
      <div class="login__split">
        <span class="login__split-line"></span>
        <span class="login__split-text">其他方式登录</span>
        <span class="login__split-line"></span>
      </div>
      <div class="login__method">
        <span class="iconfont login__method-img">&#xe66a;</span>
        <span class="iconfont login__method-img">&#xe6b3;</span>
      </div>
    </div>
  </div>
</template>

<script >

export default {
  name: 'Login',
  setup () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.login {
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
    margin-top: .36rem;
    height: .44rem;
    background-color: #c99274;
    border-radius: .44rem;
    font-size: .16rem;
    text-align: center;
    line-height: .44rem;
    color: #fff;
  }
  &__split {
    flex: 1;
    margin: .4rem 0 .3rem 0;
    display: flex;
    align-items: center;
    &-line {
      flex: 1;
      height: .02rem;
      background-color: #c99274;
    }
    &-text {
      margin: 0 .15rem;
      font-size: .12rem;
      color: #c99274;
    }
  }
  &__method {
    display: flex;
    justify-content: center;
    &-img {
      color: #c99474;
      font-size: .4rem;
      margin: 0 .2rem;
    }
  }
}
input:-webkit-autofill , textarea:-webkit-autofill, select:-webkit-autofill {
  -webkit-text-fill-color:#343434;
  box-shadow: 0 0 0px 1000px transparent inset !important;
  background-color: transparent;
  background-image: none;
  transition: background-color 50000s ease-in-out 0s;
}

</style>
