<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="container max-w-full">
    <nav class="bg-slate-900 text-white h-screen w-72 max-w-100 relative">
      <div class="w-11 h-11 absolute mt-2 ml-6 bg-slate-50 rounded-full">
        <img class="w-8 h-8 ml-1.5 mt-1.5" src="./img/P2.png" alt="" />
      </div>
      <h1 class="absolute text-white font-semibold ml-20 mt-4 text-lg">
        B.O.W PROJECT 0.1
      </h1>
      <div class="flex flex-col pt-20">
        <RouterLink
          class="px-4 mx-3 hover:bg-slate-50 hover:text-slate-800 rounded p-2"
          to="/"
          ><i class="bi bi-house-door-fill mr-2"></i>Home</RouterLink
        >
        <RouterLink
          class="px-4 mx-3 hover:bg-slate-50 hover:text-slate-800 rounded p-2"
          to="/team"
          ><i class="bi bi-people-fill mr-2"></i>Team</RouterLink
        >
        <RouterLink
          class="px-4 mx-3 hover:bg-slate-50 hover:text-slate-800 rounded p-2"
          to="/project"
          ><i class="bi bi-cast mr-2"></i>Project
        </RouterLink>
        <RouterLink
          class="px-4 mx-3 hover:bg-slate-50 hover:text-slate-800 rounded p-2"
          to="/about"
          ><i class="bi bi-grid-fill mr-2"></i>About</RouterLink
        >
      </div>
      <button
        class="hover:bg-slate-300 group absolute inset-x-0 bottom-0 flex items-center justify-center bg-white border focus:outline-none shadow text-slate-700 rounded py-2 m-2"
      >
        <img class="rounded-full w-10 h-10" src="./img/P1.jpg" alt="" />
        <p class="px-2">Jhon Khannedy</p>
        <span class="pl-10">
          <img class="w-4 h-4" src="./img/P3.svg" alt="" />
        </span>
        <div class="absolute hidden bottom-full mb-3  min-w-full w-max bg-white mt-1 rounded group-focus:block">
          <ul class="text-left border rounded">
            <li class="py-2.5 pl-2 hover:bg-slate-200 border-b"><i class="bi bi-gear-fill mr-2"></i>Setting</li>
            <li class="py-2.5 pl-2 hover:bg-slate-200 border-b"><i class="bi bi-box-arrow-right mr-2"></i>Logout</li>
          </ul>
        </div>
      </button>
      <!-- <RouterView /> -->
    </nav>
  </header>
</template>

<style scoped></style>
