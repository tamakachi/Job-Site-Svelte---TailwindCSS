<script>
  import Counter from './lib/Counter.svelte'
  import JobSite from './lib/JobSite.svelte'
</script>

<svelte:head><script src="https://cdn.tailwindcss.com"></script></svelte:head>


<main>

  <div class="w-full border-b border-gray-100 px-4">
    <div class="flex flex-row items-center max-w-7xl mx-auto justify-between  py-4">
        <div>
            <h1 class="text-3xl font-black tracking-widest text-blue-500">Job Search</h1>
        </div>

        <div class="hidden sm:grid grid-cols-2 gap-2">
            <div class="text-blue-500">Looking for</div>
            <div class="text-gray-900">
                <select class="focus:outline-none">
                    <option>job</option>
                    <option>hire</option>
                </select>
            </div>
        </div>

        <div class="hidden sm:flex gap-1 items-end">
            <svg xmlns="http://www.w3.org/2000/svg"
                 class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round"
                      d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                <path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
            </svg>
            <span class="text-gray-900 text-sm">Singapore</span>
        </div>

        <div class="hidden sm:grid grid-cols-2 place-items-end gap-2">
            <div>
                <img src="images/avatar.jpg" class="h-10 rounded-full">
            </div>
            <div class="grid grid-cols-1">
                <div class="flex items-center justify-enter gap-2">
                    <p class="text-gray-900 text-sm">David Maker</p>
                    <svg xmlns="http://www.w3.org/2000/svg"
                         class="h-3 w-3 text-gray-500"
                         viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd"
                              d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                              clip-rule="evenodd"/>
                    </svg>
                </div>
                <div>
                    <p class="text-gray-500 text-xs">Backend Developer</p>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- filter -->
<div class="w-full bg-white shadow px-4">
    <div class="max-w-7xl mx-auto grid grid-cols-1 sm:grid-cols-5 py-4 sm:divide-x sm:divide-gray-100 place-items-start sm:place-items-center gap-4 sm:gap-0">

        <div class="flex flex-row gap-2 items-center justify-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24"
                 stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/>
            </svg>
            <input class="text-gray-900 focus:outline-none p-2"
                   placeholder="search ....">
        </div>

        <div class="grid-cols-2 grid place-items-stretch place-content-stretch px-2 w-full">
            <div class="flex items-center justify-start">
                <select class="appearance-none text-gray-500 text-left w-full focus:outline-none">
                    <option>Location</option>
                </select>
            </div>
            <div class="flex items-center justify-end">
                <svg xmlns="http://www.w3.org/2000/svg"
                     class="h-3 w-3 text-gray-500"
                     viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd"
                          d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                          clip-rule="evenodd"/>
                </svg>
            </div>
        </div>

        <div class="grid-cols-2 grid place-items-stretch place-content-stretch px-2 w-full">
            <div class="flex items-center justify-start">
                <select class="appearance-none text-gray-500 text-left focus:outline-none">
                    <option>Experience</option>
                </select>
            </div>
            <div class="flex items-center justify-end">
                <svg xmlns="http://www.w3.org/2000/svg"
                     class="h-3 w-3 text-gray-500"
                     viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd"
                          d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                          clip-rule="evenodd"/>
                </svg>
            </div>
        </div>

        <div class="grid-cols-2 grid place-items-stretch place-content-stretch px-2 w-full">
            <div class="flex items-center justify-start">
                <select class="appearance-none text-gray-500 text-left focus:outline-none">
                    <option>Title</option>
                </select>
            </div>
            <div class="flex items-center justify-end">
                <svg xmlns="http://www.w3.org/2000/svg"
                     class="h-3 w-3 text-gray-500"
                     viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd"
                          d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                          clip-rule="evenodd"/>
                </svg>
            </div>
        </div>

        <div class="grid-cols-2 grid place-items-stretch place-content-stretch px-2 w-full">
            <div class="flex items-center justify-start">
                <select class="appearance-none text-gray-500 text-left focus:outline-none">
                    <option>Salary</option>
                </select>
            </div>
            <div class="flex items-center justify-end">
                <svg xmlns="http://www.w3.org/2000/svg"
                     class="h-3 w-3 text-gray-500"
                     viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd"
                          d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                          clip-rule="evenodd"/>
                </svg>
            </div>
        </div>

    </div>
</div>

<!-- content -->
<div class="max-w-7xl mx-auto grid grid-cols-1 sm:grid-cols-4 pt-10 place-items-start px-4">
    <div class="flex flex-col gap-6 items-start justify-center w-full divide-y divide-gray-100 pr-10">
        <div>
            <p class="text-2xl font-semibold">Filters</p>
        </div>

        <div class="grid grid-cols-1 divide-y divide-gray-100 w-full">
            <div class="py-4 gap-4 flex flex-col items-start justify-start">
                <h1 class="text-gray-400 font-semibold text-sm">Schedule</h1>
                <div class="flex flex-col items-start justify-center gap-2">
                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Full time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Part time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Project based</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>
                </div>
            </div>
            <div class="py-4 gap-4 flex flex-col items-start justify-start">
                <h1 class="text-gray-400 font-semibold text-sm">Employment</h1>
                <div class="flex flex-col items-start justify-center gap-2">
                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Full time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Part time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Project based</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>
                </div>
            </div>
            <div class="py-4 gap-4 flex flex-col items-start justify-start">
                <h1 class="text-gray-400 font-semibold text-sm">Locations</h1>
                <div class="flex flex-col items-start justify-center gap-2">
                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Full time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Part time</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Project based</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>

                    <label class="inline-flex flex-row items-center justify-center gap-2">
                        <input type="checkbox"
                               class="bg-blue-500 border-blue-300 focus:ring-3 focus:ring-blue-300 h-4 w-4 rounded">
                        <span>Internship</span>
                    </label>
                </div>
            </div>
        </div>

    </div>
    <div class="col-span-3 flex flex-col gap-6 items-start justify-start">
        <div class="flex items-center justify-between w-full">
            <p class="text-2xl font-semibold space-x-4"><span>Results</span> <span class="text-gray-400">600</span></p>
            <div class="flex items-center justify-start gap-2">
                <span class="text-sm text-gray-400">Sort by</span>
                <select class="text-blue-500 focus:outline-none">
                    <option>latest</option>
                    <option>salary</option>
                    <option>created</option>
                </select>
            </div>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-3 gap-2 w-full">

            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-1.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>

            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-2.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>


            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-1.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>

            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-2.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>


            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-1.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>

            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-2.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>


            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-1.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>

            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-2.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>


            <div class="flex flex-col bg-blue-50 p-4 rounded-xl">

                <div class="flex items-center justify-between pb-6">
                    <img src="images/logo-1.png" class="w-6 h-6 rounded-full">
                    <span class="text-xs text-gray-400">7 Jul 2022</span>
                </div>

                <div class="flex flex-col items-start justify-between gap-4 w-full">
                    <div class="flex items-center justify-between w-full">
                        <p class="text-2xl font-semibold truncate">UX Designer</p>
                        <span class="text-xs text-blue-500 font-semibold">20 applied</span>
                    </div>

                    <div class="flex items-center justify-start gap-2 w-full">
                        <label class="bg-purple-200 text-purple-500 px-2 py-1 text-xs rounded-2xl">Full time</label>
                        <label class="bg-green-100 text-green-300 px-2 py-1 text-xs rounded-2xl">Package</label>
                        <label class="bg-blue-100 text-indigo-500 px-2 py-1 text-xs rounded-2xl">Remot</label>
                    </div>

                    <div>
                        <h1 class="text-sm font-semibold">Web Developer</h1>
                    </div>

                    <div>
                        <p class="text-sm text-gray-500 truncate whitespace-normal">
                            Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis
                            egestas.
                        </p>
                    </div>

                    <div class="grid grid-cols-2 gap-2 w-full">
                        <a href="#" class=" px-4 rounded-xl text-white py-3 inline-flex items-center justify-center bg-blue-500">Apply</a>
                        <a href="#" class=" px-4 rounded-xl py-3 inline-flex items-center justify-center border border-gray-400 text-gray-500">Bookmark</a>
                    </div>
                </div>
            </div>

        </div>


    </div>
</div>
</main>

<style>

</style>
