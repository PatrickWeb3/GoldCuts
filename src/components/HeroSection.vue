<template>
  <div class="relative overflow-hidden">

    <main>
      <!-- Background Opacity -->
      <div 
            class="bg-black opacity-70 w-full h-full absolute"
            >
      </div>
      <div id="herobg" class="pt-10 bg-gray-900 sm:pt-16 lg:pt-8 lg:pb-14 lg:overflow-hidden bg-cover bg-center">
        <div class="mx-auto max-w-7xl lg:px-8 relative">
          <div class="lg:grid lg:grid-cols-2 lg:gap-8 lg:pl-10">
            <div class="mx-auto max-w-md px-4 sm:max-w-2xl sm:px-6 sm:text-center lg:px-0 lg:text-left lg:flex lg:items-center">
              <div class="py-48 sm:py-32 lg:py-48">
                
                <h1 class="mt-4 text-4xl tracking-tight font-extrabold text-white sm:mt-5 sm:text-6xl lg:mt-6 xl:text-6xl">
                  <span class="block">We got you covered.</span>
                  <span class="block text-indigo-400">Gold Cuts.</span>
                </h1>
                <p class="mt-3 text-base text-gray-300 sm:mt-5 sm:text-xl lg:text-lg xl:text-xl">Come learn what sets us apart from average, book an appointment below with one easy click!</p>
                <div class="mt-10 sm:mt-12">
                    <div class="">
                      <div class="mt-3 sm:mt-0 sm:ml-3">
                        <a href="https://booksy.com/en-us/390352_gold-cuts_barber-shop_18229_chicago" class="block text-center w-full py-3 px-4 rounded-md shadow bg-indigo-500 text-white font-medium hover:bg-indigo-600 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-300 focus:ring-offset-gray-900">Book Appointment Here!</a>
                      </div>
                    </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- More main page content here... -->
    </main>
  </div>
</template>

<script>

const navigation = [
  { name: 'Product', href: '#' },
  { name: 'Features', href: '#' },
  { name: 'Marketplace', href: '#' },
  { name: 'Company', href: '#' },
]

export default {
  name: 'HeroSection',
  setup() {
    return {
      navigation,
    }
  },
  
}
</script>

<style>

    #herobg {
        background-image: url("/src/static/HeroImage.jpg");
        height: 100vh;
    }

</style>