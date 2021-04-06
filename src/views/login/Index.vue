<template>
  <div class="wrapper">
    <div class="top" >
      <span :class="['top__login', { 'top__active': isLogin }]" @click="handleSwitchLogin">登录</span>
      <span :class="['top__register', { 'top__active': isRegister }]" @click="handleSwitchRegister">注册</span>
    </div>
    <Login class="content" v-if="isLogin"></Login>
    <Register class="content" v-if="isRegister"></Register>
  </div>
</template>

<script>
import { ref } from 'vue'
import Login from './Login'
import Register from './Register.vue'

export default {
  name: 'Index',
  components: { Login, Register },
  setup () {
    const isLogin = ref(true)
    const isRegister = ref(false)
    const handleSwitchLogin = () => {
      isRegister.value = false
      isLogin.value = true
    }
    const handleSwitchRegister = () => {
      isLogin.value = false
      isRegister.value = true
    }
    return { isLogin, isRegister, handleSwitchLogin, handleSwitchRegister }
  }
}
</script>

<style lang="scss" scoped>
.wrapper {
  position: absolute;
  display: flex;
  justify-content: center;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: #e3a577;
}
.top {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #ffffff;
  font-size: .18rem;
  height: .4rem;
  &__login {
    line-height: 1;
    margin-right: .6rem;
  }
  &__register {
    line-height: 1;
  }
  &__active {
    font-weight: 1000;
    font-size: .26rem;
  }
}
.content {
  position: relative;
  margin: .3rem 0rem .3rem 0rem;
  width: 80%;
}
</style>
