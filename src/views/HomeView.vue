<script setup>
import myCat from '@/assets/images/cat1.jpg';
import myCat2 from '@/assets/images/cat2.jpg';
import myCat3 from '@/assets/images/cat3.jpg';
</script>

<script>


export default {
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>
<template>
  <div class="w-full lg:w-screen h-screen bg-gray-700 flex lg:flex-row flex-col">
    <div class=" bg-gray-700 flex-shrink-0 flex lg:flex-col items-center lg:w-60 flex-row h-28">
      <div class=" bg-neutral-500 lg:mt-32 lg:ml-0 ml-5 p-10 rounded-full"></div>
      <div class="sm:hidden ml-auto mr-10" id="mobile-menu">
        <div>
          <button type="button"
            class=" relative inline-flex items-end justify-end rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
            @click="toggleMenu" :aria-expanded="isMenuOpen.toString()">
            <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
              aria-hidden="true">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
            </svg>
          </button>
          <div id="mobile-menu" :class="{ 'hidden': !isMenuOpen }"
            class=" bg-slate-800 space-y-1 px-2 pb-3 pt-2 absolute right-0 top-28 ">
            <a target="_blank" href="https://www.youtube.com/"
              class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium"
              aria-current="page">YouTube</a>
            <a target="_blank" href="https://www.google.com.tw/?hl=zh_TW"
              class=" bg-gray-900 text-gray-300  hover:text-white block rounded-md px-3 py-2 text-base font-medium">Google</a>
            <a target="_blank" href="https://www.google.com/intl/zh-TW_tw/gmail/about/"
              class=" bg-gray-900 text-gray-300 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Gmail</a>
          </div>
        </div>
      </div>

      <div class=" lg:flex-col w-full text-center justify-end lg:pr-0 pr-10 sm:flex hidden">
        <a target="_blank" href="https://www.youtube.com/" class=" text-white p-2 lg:mt-4">YouTube</a>
        <a target="_blank" href="https://www.google.com.tw/?hl=zh_TW" class=" text-white p-2 lg:mt-4">Google</a>
        <a target="_blank" href="https://www.google.com/intl/zh-TW_tw/gmail/about/"
          class=" text-white p-2 lg:mt-4">Gmail</a>
      </div>
    </div>
    <div class="grow bg-zinc-600 flex items-center w-full justify-center h-full">
      <div class="content lg:w-2/3 lg:h-3/5 md:h-4/5 h-4/5 w-full md:w-4/5">
        <div class="h-full flex md:gap-1 lg:flex-row flex-col md:flex-wrap md:flex-row lg:flex-nowrap">
          <!-- <div class="lg:w-1/3 h-full bg-zinc-300 w-full md:h-1/2 lg:h-full"></div>
          <div class="lg:w-1/3 h-full bg-zinc-200 w-full md:flex-1 md:h-1/2 lg:h-full"></div>
          <div class="lg:w-1/3 h-full bg-zinc-300 w-full md:flex-1 md:h-1/2 lg:h-full"></div> -->
          <img :src="myCat" class="lg:w-1/3 h-1/3 bg-zinc-300 w-full md:h-1/2 lg:h-full">
          <img :src="myCat2" class="lg:w-1/3 h-1/3 bg-zinc-200 md:flex-1 md:h-1/2 lg:h-full">
          <img :src="myCat3" class="lg:w-1/3 h-1/3 bg-zinc-200 md:flex-1 md:h-1/2 lg:h-full">
        </div>
      </div>
    </div>
</div></template>
