<template>
  <div class="flex justify-between min-h-screen font-sans">
    <div class="relative w-1/2 bg-cover hero">
      <div class="absolute flex justify-center w-full bottom-20">
        <div class="max-w-md text-center">
          <span class="text-3xl font-bold leading-loose text-gray-900">Control Bussiness</span>
          <p
            class="font-light leading-7 text-gray-500"
          >Dotra is the most comprehensive field service & asset managament platform with combining flexibility.</p>
          <div class="flex items-center justify-center pt-8 space-x-6">
            <button class="rounded-full focus:ring focus:ring-orange-500 focus:outline-none">
              <CircleLeft />
            </button>
            <button class="rounded-full focus:ring focus:ring-orange-500 focus:outline-none">
              <CircleRight />
            </button>
          </div>
        </div>
      </div>
    </div>

    <div class="w-1/2">
      <div class="flex flex-col px-24 pt-10">
        <LogoIcon class="self-end w-32" />
        <div class="pt-20 pb-6">
          <h1 class="text-3xl font-bold leading-loose tracking-wide">Hi, Welcome back!</h1>
          <span class="font-light text-gray-500">Login now to manage your job easely.</span>

          <div class="flex items-center justify-between pt-10 space-x-6">
            <button
              class="flex items-center justify-center w-1/2 py-4.5 rounded-lg border bg-white border-gray-400 whitespace-nowrap hover:bg-gray-50 focus:outline-none focus:ring-gray-100 focus:ring-4"
            >
              <Google class="w-6 h-6" />
              <span class="pl-3 font-medium text-gray-900">Sign in with Google</span>
            </button>
            <button
              class="flex items-center justify-center w-1/2 py-4.5 rounded-lg border bg-blue-500 whitespace-nowrap hover:bg-blue-600 focus:outline-none focus:ring-gray-100 focus:ring-4"
            >
              <Facebook class="w-6 h-6" />
              <span class="pl-3 font-medium text-white">Sign in with Facebook</span>
            </button>
          </div>

          <div class="flex items-center justify-between pt-6">
            <hr class="w-full border-gray-400" />
            <span class="px-4 font-light tracking-wider text-gray-500">or</span>
            <hr class="w-full border-gray-400" />
          </div>

          <form action>
            <div class="pt-6">
              <label for="email" class="font-light">Password</label>
              <div
                class="flex items-center w-full mt-2 transition-all border border-gray-400 rounded-lg focus-within:shadow-lg focus-within:border-orange-500"
              >
                <div class="flex items-center justify-center pl-4">
                  <Email class="w-6 h-6 pointer-events-none" />
                </div>
                <input
                  type="text"
                  name="email"
                  id="email"
                  placeholder="example@mail.com"
                  class="px-4 py-4.5 w-full focus:outline-none font-light border-0 focus:ring-0"
                />
              </div>
            </div>

            <div class="pt-6">
              <label for="password" class="font-light">Email address</label>
              <div
                class="flex items-center w-full mt-2 transition-all border border-gray-400 rounded-lg focus-within:shadow-lg focus-within:border-orange-500"
              >
                <div class="flex items-center justify-center pl-4">
                  <Lock class="w-6 h-6 pointer-events-none" />
                </div>
                <input
                  type="text"
                  name="password"
                  id="password"
                  placeholder="Enter your password"
                  class="px-4 py-4.5 w-full focus:outline-none font-light border-0 focus:ring-0"
                />
              </div>
            </div>

            <div class="flex items-center justify-between pt-4">
              <div class="flex items-center">
                <input
                  type="checkbox"
                  name="remember"
                  id="remember"
                  class="w-5 h-5 text-orange-500 bg-white border border-gray-400 rounded focus:outline-none focus:ring-orange-500"
                />
                <label for="remember" class="pl-4 font-light text-gray-900">Remember me</label>
              </div>
              <a href="#" class="text-teal-500 hover:text-teal-600">Forgot password</a>
            </div>

            <div class="pt-8">
              <button
                type="submit"
                class="w-full px-8 py-4 text-white bg-orange-500 rounded-lg shadow-lg hover:bg-orange-600 focus:ring-4 focus:ring-red-100 focus:outline-none"
              >Sign in</button>
            </div>
          </form>

          <div class="pt-4">
            <div class="font-light text-center text-gray-500">
              Not registred yet?
              <a
                href="#"
                class="font-normal text-teal-500 hover:text-teal-600"
              >Create an Account</a>
            </div>

            <div class="flex items-center justify-between pt-14">
              <span class="text-gray-500">© 2021 Dotra. All rights reserved.</span>
              <span class="flex items-center space-x-1">
                <a href="#" class="text-gray-500 hover:text-gray-600">Terms of Service</a>
                <span class="text-gray-500">&#183;</span>
                <a href="#" class="text-gray-500 hover:text-gray-600">Privacy Policy</a>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import LogoIcon from "./assets/icons/logo.vue";
import Facebook from "./assets/icons/facebook.vue";
import Google from "./assets/icons/google.vue";
import Email from "./assets/icons/email.vue";
import Lock from "./assets/icons/lock.vue";
import CircleLeft from "./assets/icons/circle-left.vue";
import CircleRight from "./assets/icons/circle-rightt.vue";
</script>
<style scoped>
.hero {
  background-image: url("./assets/images/hero.png");
}
</style>
