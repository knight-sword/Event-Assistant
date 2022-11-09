<template>
  <div class="containers">
    <div class="cont" :class="{ 's--signup': isActive }">
      <div class="form sign-in">
        <h1>Welcome back</h1>
        <v-form style="width: 300px; margin: 80px auto">
          <v-text-field label="E-mail" clearable color="primary" variant="solo"></v-text-field>
          <v-text-field label="Password" clearable color="primary" variant="solo"></v-text-field>
          <p class="forgot-pass">Forgot password?</p>
          <v-btn block color="success" size="large" type="submit"> Sign In </v-btn>
        </v-form>
        <div class="sso">
          <img class="sso_img" src="@/assets/image/fc.png" />
          <img class="sso_img" src="@/assets/image/tw1.png" />
          <img class="sso_img" src="@/assets/image/google.png" />
          <img class="sso_img" src="@/assets/image/outlook.png" />
        </div>
      </div>
      <div class="sub-cont">
        <div class="img">
          <div class="img__text m--up">
            <h2>New here?</h2>
            <p>Sign up and discover great amount of new opportunities!</p>
          </div>
          <div class="img__text m--in">
            <h2>One of us?</h2>
            <p>If you already has an account, just sign in. We've missed you!</p>
          </div>
          <div class="img__btn" @click="btnEvent">
            <span class="m--up">Sign Up</span>
            <span class="m--in">Sign In</span>
          </div>
        </div>
        <div class="form sign-up">
          <h2>Time to feel like home,</h2>
          <v-form style="width: 300px; margin: 80px auto">
            <v-text-field label="Name" clearable color="primary" variant="solo"></v-text-field>
            <v-text-field class="mb-2" clearable color="primary" label="Email" variant="solo"></v-text-field>
            <v-text-field label="Password" clearable color="primary" variant="solo"></v-text-field>
            <v-btn block color="success" size="large" type="submit"> Sign Up </v-btn>
          </v-form>

          <div class="sso">
            <img class="sso_img" src="@/assets/image/fc.png" />
            <img class="sso_img" src="@/assets/image/tw1.png" />
            <img class="sso_img" src="@/assets/image/google.png" />
            <img class="sso_img" src="@/assets/image/outlook.png" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const isActive = ref(false);
const first = ref('');
const last = ref('');
const email = ref('');
const password = ref('');
const terms = ref('');

const btnEvent = function btn() {
  isActive.value = !isActive.value;
  console.log(666);
};
</script>

<style lang="scss" scoped>
@import './login.scss';
body {
  background-color: #ededed8c !important;
}
.sso {
  height: 48px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 200px;
  margin: 0 auto;
}
.sso_img {
  width: 30px;
  height: 30px;
  float: left;
}
</style>
