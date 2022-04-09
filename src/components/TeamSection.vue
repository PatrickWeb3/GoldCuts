<template>
  <div id="BarberSection" class="bg-gray-900 lg:h-screen lg:flex bg-cover teambg">
    
    <!-- Desktop Overlay -->
    <div 
        id="teamoverlay" class="bg-black opacity-60 absolute hidden lg:block">        
    </div>

    <div class="m-auto py-12 px-4 max-w-7xl sm:px-6 lg:px-8 lg:py-24 relative">
    <!-- Mobile Overlay -->
    <div 
        id="teamoverlay" class="bg-black opacity-60 absolute top-0 left-0 lg:hidden">        
    </div>
      <div class="space-y-12 relative">
        <div class="space-y-5 sm:space-y-4 md:max-w-xl lg:max-w-3xl xl:max-w-none mx-auto">
          <h2 class="text-3xl font-extrabold text-white tracking-tight sm:text-4xl">Meet Our Barbers</h2>
          <p class="text-xl text-gray-300">Find their contacts below and make an appointment today.</p>
        </div>
        
        <ul role="list" class="space-y-4 sm:grid lg:space-y-0 lg:grid-cols-3 lg:gap-8">
          <li v-for="person in people" :key="person.name" class="py-10 px-6 bg-gray-800 text-center rounded-lg xl:px-10 xl:text-left w-96 mx-auto lg:w-full shadow-lg">
            <div class="space-y-6 xl:space-y-10">
              <img class="mx-auto h-40 w-40 rounded-full xl:w-56 xl:h-56" :src="person.imageUrl" alt="" />
              <div class="space-y-2 xl:flex xl:items-center xl:justify-between">
                <div class="font-medium text-lg leading-6 space-y-1">
                  <p class="text-indigo-400">{{ person.name }}</p>
                </div>

                <ul role="list" class="flex justify-center space-x-5">
                  <li>
                    <a :href="person.twitterUrl" class="text-gray-400 hover:text-gray-300">
                      <span class="sr-only">Twitter</span>
                      <svg class="w-5 h-5" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20">
                        <path d="M6.29 18.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0020 3.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.073 4.073 0 01.8 7.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 010 16.407a11.616 11.616 0 006.29 1.84" />
                      </svg>
                    </a>
                  </li>
                  <li>
                    <a :href="person.bookseyUrl" class="text-gray-400 hover:text-gray-300">
                      <span class="sr-only">Booksey</span>
                      <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                        <path d="M9 4.804A7.968 7.968 0 005.5 4c-1.255 0-2.443.29-3.5.804v10A7.969 7.969 0 015.5 14c1.669 0 3.218.51 4.5 1.385A7.962 7.962 0 0114.5 14c1.255 0 2.443.29 3.5.804v-10A7.968 7.968 0 0014.5 4c-1.255 0-2.443.29-3.5.804V12a1 1 0 11-2 0V4.804z"></path>
                      </svg>

                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </li>
        </ul>

      </div>
    </div>
  </div>
</template>

<script>
const people = [
  {
    name: 'Junior',
    imageUrl: require('/src/static/Junior.jpg'),
    twitterUrl: 'https://www.instagram.com/goldcuts_chicago/',
    bookseyUrl: 'https://booksy.com/en-us/390352_gold-cuts_barber-shop_18229_chicago/staffer/331840',
  },
  {
    name: 'Adrian',
    imageUrl: require('/src/static/Adrian.jpg'),
    twitterUrl: 'https://www.instagram.com/goldcuts_chicago/',
    bookseyUrl: 'https://booksy.com/en-us/390352_gold-cuts_barber-shop_18229_chicago/staffer/367500',
  },
  {
    name: 'Brandon',
    imageUrl: require('/src/static/Brandon.jpg'),
    twitterUrl: 'https://www.instagram.com/goldcuts_chicago/',
    bookseyUrl: 'https://booksy.com/en-us/390352_gold-cuts_barber-shop_18229_chicago/staffer/279719',
  },
]

export default {

  name: 'TeamSection',

  setup() {
    return {
      people,
    }
  },
}
</script>

<style>

    .teambg {
        background-image: url("/src/static/TeamBg2.jpg");
    }

    #teamoverlay {
      width: 100%;
      height: 100%; 
    }

</style>