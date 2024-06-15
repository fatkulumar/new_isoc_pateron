<template>
  <section>
    <div class="flex justify-between items-center" id="navbarStudent">
      <div class="md:w-full md:truncate md:flex justify-between items-center">
        <div class="lg:w-8/12 pt-0 md:pt-0">
          <nuxt-link to="/" class="w-full flex items-center">
            <img
              src="/navbar/logo.png"
              alt="international science olympiad contest"
              class="pt-4"
            />
          </nuxt-link>
        </div>
        <div class="mx-10 grid grid-cols-2 md:gap-7 mt-1 gap-2">
          <div
            class="bg-purple-500 flex items-center justify-center text-black border-2 border-black rounded-md py-2 md:px-16"
          >
            Competition
          </div>
          <div
            class="bg-white flex items-center justify-center text-black border-2 border-black rounded-md py-2"
          >
            FAQ
          </div>
          <div
            class="bg-green-400 flex items-center justify-center text-white border-2 border-black rounded-md py-2"
          >
            Practice
          </div>
          <div
            class="bg-green-500 flex items-center justify-center text-white border-2 border-black rounded-md py-2"
          >
            Contact Us
          </div>
        </div>
        <div class="pb-2 mb-5">
          <nuxt-link to="/" class="flex items-center">
            <button
              class="px-32 py-2 mt-3 border-2 border-black border-collapse rounded-md text-white bg-purple-500 w-full"
            >
              Login
            </button>
          </nuxt-link>
          Don't have an account yet ?
          <nuxt-link to="/" class="flex items-center">
            <button
              class="px-6 border-2 border-black border-collapse rounded-md text-black bg-purple-300 w-full py-2 md:py-0 md:w-7/12"
            >
              Register
            </button>
          </nuxt-link>
        </div>
      </div>
    </div>
    <div
      class="bg-red-100 flex justify-center items-center md:justify-around p-8 flex-col md:flex-row"
    >
      <a href="" class="hover:underline"> About </a>
      <a href="" class="hover:underline"> Category </a>
      <a href="" class="hover:underline"> Benefit </a>
      <a href="" class="hover:underline"> Announcements </a>
      <a href="" class="hover:underline"> Syilabus </a>
      <a href="" class="hover:underline"> Tutorial </a>
    </div>
  </section>
</template>
  
  <style>
.dropdown:focus-within .dropdown-menu {
  opacity: 1;
  transform: translate(0) scale(1);
  visibility: visible;
}

ul {
  list-style: none;
  padding: 0;
}

.dropdown-navbar {
  top: 55px;
}

.active {
  /*fill: #fd7d00 !important;*/
}

@media screen and (max-width: 640px) {
  .dropdown-navbar {
    right: -30px;
  }
}

#competitionSubMenu {
  position: absolute;
  z-index: 999;
  top: 48px;
  width: 140px;
}

.language-dropdown {
  position: relative;
}

.language-dropdown img {
  cursor: pointer;
}

.dropdown-content {
  position: absolute;
  top: 100%;
  left: 0;
  display: none;
  background-color: #fff;
  padding: 10px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content li {
  cursor: pointer;
  margin-bottom: 5px;
}

.language-dropdown:hover .dropdown-content {
  display: block;
}
</style>
  