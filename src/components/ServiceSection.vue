<template>
  <div class="bg-indigo-500 lg:py-32">
    <section aria-labelledby="features-heading" class="relative">
      
      <div class="aspect-w-3 aspect-h-2 overflow-hidden sm:aspect-w-5 lg:aspect-none lg:absolute lg:w-1/2 lg:h-full lg:p-10 lg:pl-12 xl:pl-20 2xl:pl-32">
        <img :src='require(`/src/static/ServiceSection.jpg`)' class="h-full w-full object-center object-cover lg:h-full lg:w-full lg:rounded-lg mt-5 lg:m-0" />
      </div>

      <div class="max-w-2xl mx-auto pt-16 pb-24 px-4 sm:pb-32 sm:px-6 lg:max-w-7xl lg:pt-32 lg:px-8 lg:grid lg:grid-cols-2 lg:gap-x-8">
        <div class="lg:col-start-2">
          <p class="mt-4 text-4xl font-extrabold text-gray-100 tracking-tight">Barber Services</p>
          <p class="mt-4 text-indigo-200 font-bold">Come in and enjoy a great haircut, leave with a Golden Crisp!</p>

          <dl class="mt-10 grid grid-cols-1 gap-y-10 gap-x-8 text-sm">
            <div v-for="feature in features" :key="feature.name">
              <dt class="font-bold text-white">{{ feature.name }}</dt>
              <dd class="mt-2 text-indigo-200">{{ feature.description1 }} <span class="text-gray-100 font-bold">{{ feature.price1}}</span></dd>
              <dd class="mt-2 text-indigo-200">{{ feature.description2 }} <span class="text-gray-100 font-bold">{{ feature.price2}}</span></dd>
            </div>
          </dl>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
const features = [
  {
    name: 'Popular Services',
    description1: 'Barber Hair Cut (hair lining now included) -',
    price1: '$25',
    description2: 'Seniors, kids, military and buzz cut w/ no line up -',
    price2: '$18',
  },
  {
    name: 'Other Services',
    description1: 'Barber Hair Cut (hair lining now included) -',
    price1: '$25',
    description2: 'Seniors, kids, military and buzz cut w/ no line up -',
    price2: '$18',
  }
]

export default {

  name: 'ServiceSection',  

  setup() {
    return {
      features,
    }
  },
}
</script>