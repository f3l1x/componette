<template>
  <div>
    <header class="px-2 bg-gradient-r-blue-900-blue-700 md:px-4 relative">
      <div class="container z-10 relative flex items-center justify-between pb-8 mx-auto lg:pb-10">
        <a href="/" class="flex items-center pt-2 pb-1 text-sm font-bold text-white uppercase md:pt-3 md:pb-2 md:text-base xl:text-xl group focus:outline-none">
          <img loading="lazy" src="/logo.svg" class="h-12 w-12 mr-2 md:h-16 md:w-16 transform transition-all duration-300 ease-in-out group-hover:rotate-360" />
          <h1>Componette</h1>
        </a>
        <div x-data="{ open: false }" class="relative flex-shrink-0 md:flex-1">
          <button x-on:click="open = true" class="p-2 rounded focus:outline-none hover:bg-blue-800 transition duration-150 ease-in-out md:hidden" x-bind:class="{ 'bg-blue-800': open }">
            <div class="relative flex w-6 h-6">
              <img loading="lazy" src="https://obr.now.sh/remixicon/system/menu-line/64/ffffff" class="absolute w-6 h-6" x-bind:class="{ hidden: open }" />
              <img loading="lazy" src="https://obr.now.sh/remixicon/system/close-line/64/ffffff" class="absolute w-6 h-6" x-bind:class="{ hidden: !open }" />
            </div>
            <span class="hidden">Open mobile menu</span>
          </button>
          <ul
            x-transition:enter="transition ease-out duration-150"
            x-transition:enter-start="opacity-0 transform scale-75"
            x-transition:enter-end="opacity-100 transform scale-100"
            x-transition:leave="transition ease-in duration-150"
            x-transition:leave-start="opacity-100 transform scale-100"
            x-transition:leave-end="opacity-0 transform scale-75"
            x-on:click.away="open = false"
            class="absolute right-0 z-20 items-center w-32 py-2 mt-2 bg-white rounded shadow-md transform origin-top-right md:mt-0 md:bg-transparent md:shadow-none md:relative md:flex md:flex-1 md:w-auto md:text-right top-menu"
          >
            <li class="md:inline-flex">
              <a href="/" class="flex px-4 py-2 text-xs hover:bg-blue-100 md:hover:bg-blue-800 md:rounded md:hover:text-blue-200 md:text-blue-400 md:text-sm transition duration-150 ease-out focus:outline-none">Planette</a>
            </li>
            <li class="md:inline-flex">
              <a href="/" class="flex px-4 py-2 text-xs hover:bg-blue-100 md:hover:bg-blue-800 md:rounded md:hover:text-blue-200 md:text-blue-400 md:text-sm transition duration-150 ease-out focus:outline-none">Forum</a>
            </li>
            <li class="md:inline-flex">
              <a href="/" class="flex px-4 py-2 text-xs hover:bg-blue-100 md:hover:bg-blue-800 md:rounded md:hover:text-blue-200 md:text-blue-400 md:text-sm transition duration-150 ease-out focus:outline-none">Blog</a>
            </li>
            <li class="md:inline-flex">
              <a href="/" class="flex px-4 py-2 text-xs hover:bg-blue-100 md:hover:bg-blue-800 md:rounded md:hover:text-blue-200 md:text-blue-400 md:text-sm transition duration-150 ease-out focus:outline-none">Donate</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="absolute z-0 left-0 top-0 h-full w-full overflow-hidden" aria-label="hidden">
        <div class="grid grid-cols-12 grid-rows-1 max-w-sm lg:max-w-lg xl:max-w-6xl mx-auto">
          <div class="col-start-3 xl:col-start-2 row-start-1 col-2 relative">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-700 opacity-25 transform xl:-translate-y-1/2 -ml-48 md:-ml-96 -mt-48 xl:-ml-128 xl:-mt-24 w-64 xl:w-96">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
          </div>
          <div class="col-start-3 xl:col-start-2 row-start-1 col-2 relative">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-700 opacity-25 transform xl:-translate-y-1/2 -ml-64 md:-ml-72 -mt-48 xl:-ml-96 xl:-mt-24 w-64 xl:w-96">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
          </div>
          <div class="col-start-10 xl:col-start-11 row-start-1 col-2 relative">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-600 opacity-25 transform translate-y-8 translate-x-24 translate-y-10 w-32 md:w-96">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
          </div>
          <div class="col-start-10 xl:col-start-11 row-start-1 col-2 relative">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-600 opacity-25 transform translate-x-64 translate-y-16 w-32 md:w-64">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
          </div>
          <div class="col-start-10 xl:col-start-11 row-start-1 col-2 relative">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-600 opacity-25 transform translate-x-72 -translate-y-16 md:w-32">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
          </div>
        </div>
      </div>
    </header>
    <div class="px-2 -mb-4 md:px-4 md:-mb-1 lg:-mb-0">
      <div class="container flex mx-auto bg-white rounded shadow-xl transform -translate-y-1/2">
        <input type="text" class="flex-1 w-full px-5 py-4 text-sm border-0 lg:px-8 lg:py-6 form-input md:text-base focus:outline-none" placeholder="Datagrid, tracy, doctrine, database, latte…" />
        <button type="submit" class="inline-flex items-center flex-shrink-0 px-4 text-sm font-medium text-blue-700 uppercase rounded-r md:px-8 xl:text-base transition duration-150 ease-in-out hover:bg-blue-100 focus:outline-none">
          <img loading="lazy" src="https://obr.now.sh/remixicon/system/search-line/64/8A99B0" class="h-5 md:mr-4" />
          <span class="hidden md:block">Search</span>
        </button>
      </div>
    </div>
  </div>
</template>
