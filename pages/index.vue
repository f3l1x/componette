<template>
  <div>
    <div class="px-2 md:px-4 overflow-hidden">
      <div class="container mx-auto">
        <div class="grid grid-cols-3 gap-4 mb-4">
          <div class="order-2 row-span-3 col-span-3 lg:col-span-2 lg:order-1 relative z-0">
            <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-200 absolute bottom-0 left-0 z-0 w-24 transform -mb-2 -ml-4 -translate-x-1/2 translate-y-1/2">
              <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
            </svg>
            <div class="bg-white rounded shadow-md z-10 relative">
              <div class="flex flex-wrap items-center justify-between px-5 pt-3 lg:px-8 lg:pt-4">
                <div class="mb-3 lg:mb-5">
                  <h2 class="text-xl font-bold text-gray-800 lg:text-3xl font-headers">Latest updated addons</h2>
                  <p class="text-sm text-blue-700">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                </div>
                <a href="/" class="inline-flex px-4 py-2 mb-3 font-medium text-teal-900 uppercase border rounded lg:mb-4 hover:bg-blue-100 transition duration-150 ease-in-out">Show all</a>
              </div>
              <div v-for="item in 5" :key="item" class="flex flex-wrap items-center justify-between px-5 pt-3 border-t lg:px-8 lg:pt-4">
                <div class="flex items-center w-full mb-3 lg:mb-5 md:w-3/5">
                  <a href="/detail" class="flex-shrink-0 mr-4">
                    <img loading="lazy" src="https://avatars.githubusercontent.com/contributte?s=128" class="w-8 h-8 rounded-full lg:h-16 lg:w-16" />
                  </a>
                  <div class="flex flex-col flex-1">
                    <h3 class="inline-block mb-2 text-lg font-bold leading-tight text-teal-800 font-headers xl:text-xl align-middle">
                      <a href="/detail" class="mr-2">contributte / foo</a> <span class="relative inline-block px-2 text-sm font-normal text-blue-700 bg-blue-100 rounded-full -mt-1 align-middle">1.2.3</span>
                    </h3>
                    <p class="text-sm text-gray-700">Example package.</p>
                  </div>
                </div>
                <div class="flex flex-wrap w-full pl-12 sm:w-4/5 md:pl-4 md:w-2/5">
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/system/download-cloud-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/system/star-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/weather/flashlight-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="order-1 col-span-3 grid grid-cols-2 gap-2 lg:col-span-1">
            <a href="/" class="col-span-2 inline-flex items-center justify-center px-5 py-3 text-gray-200 uppercase rounded w-full lg:py-4 bg-gradient-l-blue-900-blue-700 hover:bg-blue-900 hover:text-white hover:bg-no-image">
              <img loading="lazy" src="https://obr.now.sh/remixicon/system/add-circle-line/64/8A99B0" class="h-5 mr-2" />
              <span>Add new package</span>
            </a>
            <div class="grid grid-cols-2 gap-2 col-span-2">
              <a href="/" class="inline-flex text-xs md:text-sm items-center justify-center px-2 py-2 text-teal-200 uppercase rounded flex-1 bg-teal-700 hover:bg-teal-800 hover:text-white transition duration-150 ease-in-out">
                <img loading="lazy" src="https://obr.now.sh/remixicon/system/dashboard-line/64/88CEDA" class="h-5 mr-2" />
                <span>Form builder</span>
              </a>
              <a href="/" class="inline-flex text-xs md:text-sm items-center justify-center px-2 py-2 font-medium text-gray-900 uppercase flex-1 bg-white rounded hover:bg-blue-200 transition duration-150 ease-in-out">
                <span>All packages</span>
              </a>
            </div>
          </div>
          <div class="order-3 col-span-3 lg:col-span-1 z-10">
            <div class="bg-teal-200 rounded shadow-md">
              <div class="bg-orange-500 text-sm font-bold leading-tight py-1 uppercase text-white inline-flex items-center rounded-r pl-5 pr-2 lg:pl-8 mt-3 lg:mt-4">
                <img loading="lazy" src="https://obr.now.sh/remixicon/weather/blaze-line/64/ffffff" class="w-4 h-4 mr-2" />Hot
              </div>
              <div class="relative">
                <div class="px-5 pt-3 lg:px-8 lg:pt-4 text-teal-800">
                  <h2 class="text-lg mb-2 font-bold font-headers text-teal-900 lg:text-xl">Componette is great</h2>
                  <p class="mb-3 lg:mb-5">
                    Take a look and say hey! Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Nullam justo enim, consectetuer nec, ullamcorper ac, vestibulum in, elit. Proin mattis lacinia justo. Phasellus rhoncus. Donec quis nibh
                    at felis congue commodo. Morbi leo mi, nonummy eget tristique non, rhoncus non leo. In convallis. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Curabitur
                    sagittis hendrerit ante. Nulla est. Sed convallis magna eu sem. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos hymenaeos. Pellentesque arcu. Cum sociis natoque penatibus et magnis dis
                    parturient montes, nascetur ridiculus mus. Nulla non arcu lacinia neque faucibus fringilla. In rutrum. Nulla non arcu lacinia neque faucibus fringilla.
                  </p>
                </div>
                <div class="absolute bg-gradient-b-transparent-teal-200 bottom-0 left-0 w-full h-32 pointer-events-none" aria-label="hidden"></div>
              </div>
              <div class="flex flex-wrap items-center justify-between px-5 lg:px-8 pb-3 lg:pb-4">
                <span class="mb-3 lg:mb-4 text-sm mr-2 font-medium text-teal-800">1.1.2021</span>
                <a href="/" class="inline-flex px-4 py-2 mb-3 font-medium text-teal-800 uppercase border border-teal-300 rounded lg:mb-4 bg-white hover:bg-teal-100 transition duration-150 ease-in-out">Read more</a>
              </div>
            </div>
          </div>
        </div>
        <div class="grid grid-cols-3 gap-4">
          <div class="order-2 row-span-3 col-span-3 lg:col-span-2 lg:order-1 relative z-10">
            <div class="bg-white rounded shadow-md lg:mb-4">
              <div class="flex flex-wrap items-center justify-between px-5 pt-3 lg:px-8 lg:pt-4">
                <div class="mb-3 lg:mb-5">
                  <h2 class="text-xl font-bold text-gray-800 lg:text-3xl font-headers">Latest indexed addons</h2>
                  <p class="text-sm text-blue-700">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                </div>
                <a href="/" class="inline-flex px-4 py-2 mb-3 font-medium text-teal-900 uppercase border rounded lg:mb-4 hover:bg-blue-100 transition duration-150 ease-in-out">Show all</a>
              </div>
              <div v-for="item in 15" :key="item" class="flex flex-wrap items-center justify-between px-5 pt-3 border-t lg:px-8 lg:pt-4">
                <div class="flex items-center w-full mb-3 lg:mb-5 md:w-3/5">
                  <a href="/detail" class="flex-shrink-0 mr-4">
                    <img loading="lazy" src="https://avatars.githubusercontent.com/contributte?s=128" class="w-8 h-8 rounded-full lg:h-16 lg:w-16" />
                  </a>
                  <div class="flex flex-col flex-1">
                    <h3 class="inline-block mb-2 text-lg font-bold leading-tight text-teal-800 font-headers xl:text-xl align-middle">
                      <a href="" class="mr-2">contributte / foo</a> <span class="relative inline-block px-2 text-sm font-normal text-blue-700 bg-blue-100 rounded-full -mt-1 align-middle">1.2.3</span>
                    </h3>
                    <p class="text-sm text-gray-700">Example package.</p>
                  </div>
                </div>
                <div class="flex flex-wrap w-full pl-12 sm:w-4/5 md:pl-4 md:w-2/5">
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/system/download-cloud-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/system/star-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                  <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                    <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                      <img loading="lazy" src="https://obr.now.sh/remixicon/weather/flashlight-fill/64/467A85" class="w-4 h-4" />
                    </div>
                    123456
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="order-3 col-span-3 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-1 gap-4 lg:col-span-1">
            <div class="relative">
              <div class="bg-white rounded shadow-md relative z-10">
                <div class="flex flex-wrap items-center justify-start px-5 pt-3 lg:px-8 lg:pt-4">
                  <img loading="lazy" src="i_trophy.svg" class="rounded-full w-8 h-8 p-1 border mb-3 lg:mb-5 mr-4 flex-shrink-0" />
                  <div class="mb-3 lg:mb-5 flex-1">
                    <h2 class="text-lg font-bold text-gray-800 lg:text-2xl font-headers">Package of the month</h2>
                  </div>
                </div>
                <div class="flex flex-wrap items-center justify-between px-5 pt-3 border-t lg:px-8 lg:pt-4">
                  <div class="flex items-start w-full mb-3 lg:mb-5">
                    <a href="" class="flex-shrink-0 mr-4">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/slevomat?s=128" class="w-8 h-8 rounded-full" />
                    </a>
                    <div class="flex flex-col flex-1">
                      <h3 class="inline-block mb-2 text-base font-bold leading-tight text-teal-800 font-headers xl:text-lg align-middle">
                        <a href="" class="inline-block mr-2 hover:underline">tacoberu / nette-mailing</a> <span class="relative inline-block px-2 text-sm font-normal text-blue-700 bg-blue-100 rounded-full -mt-1 align-middle">3.2.0</span>
                      </h3>
                      <p class="text-sm text-gray-700">Support send mail in nette application.</p>
                    </div>
                  </div>
                  <div class="flex flex-wrap w-full pl-12 sm:w-4/5 sm:pl-4">
                    <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                      <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                        <img loading="lazy" src="https://obr.now.sh/remixicon/system/download-cloud-fill/64/467A85" class="w-4 h-4" />
                      </div>
                      481
                    </div>
                    <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                      <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                        <img loading="lazy" src="https://obr.now.sh/remixicon/system/star-fill/64/467A85" class="w-4 h-4" />
                      </div>
                      481
                    </div>
                    <div class="flex items-center flex-1 mb-3 text-xs text-blue-700 lg:mb-5 md:justify-end">
                      <div class="inline-flex items-center justify-center w-6 h-6 mr-2 bg-teal-100 rounded-full">
                        <img loading="lazy" src="https://obr.now.sh/remixicon/weather/flashlight-fill/64/467A85" class="w-4 h-4" />
                      </div>
                      481
                    </div>
                  </div>
                </div>
              </div>
              <svg fill="currentColor" viewBox="0 0 100 100" class="text-blue-200 absolute top-0 lg:top-auto lg:bottom-0 right-0 z-0 w-24 transform -mb-2 -mr-2 lg:-mr-4 translate-x-1/2 -translate-y-1/2 lg:translate-y-1/2">
                <path id="Path_236" d="M12.9,24.2c-2.2,1.4-3.6,3.8-3.7,6.4v38.7c0.1,2.6,1.5,5,3.7,6.4L46.3,95c2.3,1.2,5.1,1.2,7.4,0l33.4-19.3 c2.2-1.4,3.6-3.8,3.7-6.4V30.6c-0.1-2.6-1.5-5-3.7-6.4L53.8,5c-2.3-1.2-5.1-1.2-7.4,0L12.9,24.2z" />
              </svg>
            </div>
            <div class="relative">
              <div class="bg-white rounded shadow-md mb-4">
                <div class="flex flex-wrap items-center justify-start px-5 pt-3 lg:px-8 lg:pt-4">
                  <img loading="lazy" src="i_merge.svg" class="rounded-full w-8 h-8 p-1 border mb-3 lg:mb-5 mr-4 flex-shrink-0" />
                  <div class="mb-3 lg:mb-5 flex-1">
                    <h2 class="text-lg font-bold text-gray-800 lg:text-2xl font-headers">Latest updated addons</h2>
                  </div>
                </div>
                <div class="flex flex-col flex-wrap justify-start px-5 pt-4 border-t lg:px-8 lg:pt-6 pb-2 lg:pb-4">
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">ninjify/coding-standard</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">nextras/tracy-monolog-adapter</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">nexendrie/translation</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">contributte/codeception</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">ninjify/coding-standard</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">nextras/tracy-monolog-adapter</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">nexendrie/translation</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                  <a href="" class="flex flex-wrap items-center mb-2 justify-between leading-tight text-teal-800 group">
                    <span class="inline-flex items-center text-sm font-medium font-headers">
                      <img loading="lazy" src="https://avatars.githubusercontent.com/nextras?s=128" class="w-3 h-3 rounded-full flex-shrink-0 mr-1" />
                      <span class="flex-1 group-hover:underline">contributte/codeception</span>
                    </span>
                    <span class="relative inline-block px-2 text-xs font-normal text-blue-700 bg-blue-100 rounded-full align-middle leading-tight">3.2.0</span>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="px-2 md:px-4">
      <div class="container mx-auto pb-2">
        <div class="px-3 lg:px-6">
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-600 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> api </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-600 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> forms </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-600 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> utils </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-400 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> api </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-400 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> forms </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-red-400 text-red-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> utils </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-yellow-600 text-yellow-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> component </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-yellow-600 text-yellow-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> database </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-yellow-300 text-yellow-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> component </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-yellow-300 text-yellow-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> database </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-purple-600 text-purple-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> tracy </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-purple-600 text-purple-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> doctrine </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-purple-200 text-purple-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> tracy </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-purple-200 text-purple-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> doctrine </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-blue-600 text-blue-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> tracy </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-blue-600 text-blue-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> doctrine </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-blue-200 text-blue-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> tracy </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-blue-200 text-blue-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> doctrine </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-600 text-green-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> security </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-600 text-green-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> extension </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-600 text-green-100 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> latte </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-200 text-green-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> security </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-200 text-green-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> extension </span>
          </div>
          <div class="bg-white inline-flex items-center rounded mb-2 mx-2 text-sm">
            <span class="bg-green-200 text-green-800 rounded-l py-1 px-2"> 75 </span>
            <span class="py-1 px-2 text-gray-800"> latte </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
