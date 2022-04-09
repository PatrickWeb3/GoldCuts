<template>
  <div class="bg-gray-100 h-max py-32 lg:py-56" id="ContactSection">
    <div class="flex flex-col justify-center items-center h-full">

      <div class="max-w-7xl mx-auto px-4 sm:px-6 md:mb-10 lg:px-8">
        <div class="lg:text-center">
          <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl mb-3">Gold Cuts Barber Shop</p>
          <h2 class="text-base text-indigo-600 font-semibold tracking-wide uppercase">Barbers of Chicago</h2>
        </div>
      </div>

      <div class="flex flex-col md:flex-row max-w-2xl mx-auto">
        <div class="max-w-7xl m-auto py-10 px-4 sm:pb-5 md:pb-10 sm:px-6 lg:px-8 md:mr-20">
          <h2 class="text-3xl font-extrabold text-gray-900">Hours</h2>
          <div class="mt-5 flex flex-col">
            <div class="mb-5">
              <h3 class="text-lg font-medium text-gray-900">Monday-Saturday:</h3>
              <p class="mt-2 text-base text-gray-500">
                <span class="block">09:30am-6:30pm</span>
                <span class="block">08:00am-5:30pm</span>
              </p>
            </div>
            <div>
              <h3 class="text-lg font-medium text-gray-900">Sunday:</h3>
              <p class="mt-2 text-base text-gray-500">
                <span class="block">Always</span>
                <span class="block">Closed</span>
              </p>
            </div>
          </div>
        </div>

        <div class="max-w-7xl m-auto lg:py-10 px-4 sm:py-5 sm:px-6 lg:px-8">
          <h2 class="text-3xl font-extrabold text-gray-900">Location</h2>
          <div class="mt-5 flex flex-col">
            <div class="mb-5">
              <h3 class="text-lg font-medium text-gray-900">Address:</h3>
              <p class="mt-2 text-base text-gray-500">
                <span class="block">4141 N Broadway St.</span>
                <span class="block">Chicago, IL 60613</span>
              </p>
            </div>
            <div>
              <h3 class="text-lg font-medium text-gray-900">Phone:</h3>
              <p class="mt-2 text-base text-gray-500">
                <span class="block">(312)-783-5812</span>
                <span class="block">(312)-264-5352</span>
              </p>
            </div>
          </div>
        </div>

      </div>
    </div>


  </div>
</template>

<script>
export default {

  name: 'ContactSection',  

  setup() {
    return {
    }
  },
}
</script>