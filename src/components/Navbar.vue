<template>
<nav class="bg-sky-400 border-gray-200 px-2 sm:px-4 py-2.5 rounded border-b-2 border-sky-800">
  <div class="container flex justify-between items-center px-60 py-5">
    <div class="flex">
        <a href="#" class="flex items-center pr-10">
            <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">Toko Hape</span>
        </a>
            <div class="relative w-20 group text-black pt-1">
                <div class="text-white">
                    Menu
                </div>
                <div class="hovering absolute invisible group-hover:visible bg-white">
                    <div class="relative group2 bg-white">
                        <div class="py-2">
                            Cat & Perlengkapan
                        </div>
                        <div class="hovering2 absolute invisible group2-hover:visible bg-white text-black">
                            <ul class="hover2">
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            </ul>
                        </div>
                    </div>

                    <div class="relative group2 bg-white">
                        <div class="py-2">
                            Cat & Perlengkapan
                        </div>
                        <div class="hovering2 absolute invisible group2-hover:visible bg-white text-black">
                            <ul class="hover2">
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            </ul>
                        </div>
                    </div>

                    <div class="relative group2 bg-white">
                        <div class="py-2">
                            Cat & Perlengkapan
                        </div>
                        <div class="hovering2 absolute invisible group2-hover:visible bg-white text-black">
                            <ul class="hover2">
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            <li class="p-3">Cat Tembok</li>
                            <li class="p-3">Cat Kayu</li>
                            <li class="p-3">Semen Acian</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
    </div>
  <div class="flex md:order-1">
    <button type="button" data-collapse-toggle="mobile-menu-3" aria-controls="mobile-menu-3" aria-expanded="false" class="md:hidden text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 mr-1" >
      <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd"></path></svg>
    </button>
    <div class="hidden relative md:block">
      <div class="flex absolute inset-y-0 left-0 items-center pl-3 pointer-events-none">
        <svg class="w-5 h-5 text-gray-500" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd"></path></svg>
      </div>
      <input type="text" id="search-navbar" class="search-bars block p-2 pl-10 w-full text-gray-900 bg-white rounded-lg border border-gray-300 sm:text-sm focus:ring-blue-500 focus:border-blue-500 dark:bg-white dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Search...">
    </div>
    <button data-collapse-toggle="mobile-menu-3" type="button" class="inline-flex items-center p-2 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu-3" aria-expanded="false">
    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
    </button>
  </div>
    <div class="hidden justify-between items-center w-full md:flex md:w-auto md:order-1" id="mobile-menu-3">
      <div class="relative mt-3 md:hidden">
        <div class="flex absolute inset-y-0 left-0 items-center pl-3 pointer-events-none">
          <svg class="w-5 h-5 text-gray-500" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd"></path></svg>
        </div>
        <input type="text" id="search-navbar" class="block p-2 pl-10 w-full text-gray-900 bg-gray-50 rounded-lg border border-gray-300 sm:text-sm focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Search...">
      </div>
      <ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium">
        <li>
          <a href="#" class="rounded-full bg-white text-black px-3 py-2">Sign Up</a>
        </li>
        <li>
            <a href="#" class="rounded-full bg-white text-black px-3 py-2">Sign In</a>
        </li>
        <li>
            <a href="#" class="text-white px-3 py-2">Cart</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>

<style lang="scss">
.hovering {
    z-index: 100;
    text-align: left;
    padding: 2rem;
    width: 15rem;
}

.hovering2 {
    left: 13rem;
    top: 0;
    width: 25rem;
}

.hover2 {
        display: grid;
    grid-template-rows: repeat(3, min-content);
    grid-auto-flow: column;
}

.group:hover .group-hover\:visible {
  visibility: visible;
}

.group2:hover .group2-hover\:visible {
  visibility: visible;
}

.left-20 {
  left: 5rem;
}

.search-bars {
    width: 30rem;
}
</style>