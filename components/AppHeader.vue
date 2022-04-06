<template>
  <div class="border-b-2 border-gray-100">
    <div class="container mx-auto">
      <nav class="flex bg-teal-500 p-6">
        <div class="flex items-center flex-shrink-0 text-white mr-6">
          <img src="/logo.png">
        </div>
        <div class="block lg:hidden">
          <button class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white">
            <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" /></svg>
          </button>
        </div>
        <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
          <div class="text-sm">
            <a href="#responsive-header" class="block mt-4 lg:inline-block lg:mt-0 text-gray-600 hover:underline mx-2">
              HOME
            </a>
            <button type="button" class="group bg-white rounded-md inline-flex items-center text-gray-600" aria-expanded="false">
              <span>ART</span>
              <svg class="text-gray-400 h-5 w-5 group-hover:text-gray-500" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
              </svg>
            </button>

            <a href="#responsive-header" class="block mt-4 lg:inline-block lg:mt-0 text-gray-600 hover:underline mx-2">
              FOR ARTISTS
            </a>
            <a href="#responsive-header" class="block mt-4 lg:inline-block lg:mt-0 text-gray-600 hover:underline  mx-2">
              BLOG
            </a>
          </div>
        </div>
        <div class="grow" />
        <div class="hidden md:flex items-center justify-end md:flex-1 lg:w-0">
          <button class="bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
            <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M13 8V2H7v6H2l8 8 8-8h-5zM0 18h20v2H0v-2z" /></svg>
          </button>
        </div>
      </nav>
    </div>
  </div>
</template>

<style>
</style>
