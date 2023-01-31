<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="container max-w-full">
    <nav class="relative h-screen text-white bg-slate-900 w-72 max-w-100">
      <div class="absolute mt-3 ml-6 text-center ">
        <img class="w-10 h-10 p-1 rounded-full bg-slate-50" src="./img/P2.png" alt="" />
      </div>
      <h1 class="absolute mt-5 ml-20 text-lg font-semibold text-white">
        B.O.W PROJECT 0.1
      </h1>
      <div class="flex flex-col pt-20">
        <RouterLink
          class="p-2 px-4 mx-3 rounded hover:bg-slate-50 hover:text-slate-800"
          to="/"
          ><i class="mr-2 bi bi-house-door-fill"></i>Home</RouterLink
        >
        <RouterLink
          class="p-2 px-4 mx-3 rounded hover:bg-slate-50 hover:text-slate-800"
          to="/team"
          ><i class="mr-2 bi bi-people-fill"></i>Team</RouterLink
        >
        <RouterLink
          class="p-2 px-4 mx-3 rounded hover:bg-slate-50 hover:text-slate-800"
          to="/project"
          ><i class="mr-2 bi bi-cast"></i>Project
        </RouterLink>
        <RouterLink
          class="p-2 px-4 mx-3 rounded hover:bg-slate-50 hover:text-slate-800"
          to="/about"
          ><i class="mr-2 bi bi-grid-fill"></i>About</RouterLink
        >
      </div>
      <button
        class="absolute inset-x-0 bottom-0 flex items-center justify-center py-2 m-2 bg-white border rounded shadow hover:bg-slate-300 group focus:outline-none text-slate-700"
      >
        <img class="w-10 h-10 rounded-full" src="./img/P1.jpg" alt="" />
        <p class="px-2">Jhon Khannedy</p>
        <span class="pl-10">
          <img class="w-4 h-4" src="./img/P3.svg" alt="" />
        </span>
        <div class="absolute hidden min-w-full mt-1 mb-3 bg-white rounded bottom-full w-max group-focus:block">
          <ul class="text-left border rounded">
            <li class="py-2.5 pl-2 hover:bg-slate-200 border-b"><i class="mr-2 bi bi-gear-fill"></i>Setting</li>
            <li class="py-2.5 pl-2 hover:bg-slate-200 border-b"><i class="mr-2 bi bi-box-arrow-right"></i>Logout</li>
          </ul>
        </div>
      </button>
    </nav>
  </header>
  <RouterView class="inset-0 h-10 pt-2 pl-2 bg-slate-200 ml-72 text-slate-800" />
</template>

<style scoped></style>
