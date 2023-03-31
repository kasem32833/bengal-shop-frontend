<template>
  <div>

    <!-- <vue-slick-carousel :arrows="true" :dots="true">
      <div>1</div>
      <div>2</div>
      <div>3</div>
      <div>4</div>
    </vue-slick-carousel> -->


    <div class="p-8 relative">
      <vue-slick-carousel :arrows="false" :dots="true">
        <div class="slide-bg rounded-2xl pt-8">
          <div class="container">
            <div class="flex items-center ">
              <div class="w-1/2 mr-6 font-size-22">
                <p class="bs-dark-green-color font-size-32 mb-4">Save up to 30% off</p>
                <h2 class="text-6xl font-bold mb-6 text-gray-800">Bengal Vegetable Farm  Organic 100%</h2>
                <p class="mb-8">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vehicula faucibus massa est elit maecenas.</p>
                <nuxt-link to="" class="bs-button text-base">Shop now</nuxt-link>
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="500" src="~/assets/img/hero.png" alt="">
              </div>
            </div>
          </div>
        </div>

        <div class="slide-bg rounded-2xl pt-8">
          <div class="container">
            <div class="flex items-center ">
              <div class="w-1/2 mr-6 font-size-22">
                <p class="bs-dark-green-color font-size-32 mb-4">Save up to 40% off</p>
                <h2 class="text-6xl font-bold mb-6 text-gray-800">Bengal Vegetable Farm  Organic 100%</h2>
                <p class="mb-8">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vehicula faucibus massa est elit maecenas.</p>
                <nuxt-link to="" class="bs-button text-base">Shop now</nuxt-link>
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="500" src="~/assets/img/hero.png" alt="">
              </div>
            </div>
          </div>
        </div>

        <div class="slide-bg rounded-2xl pt-8">
          <div class="container">
            <div class="flex items-center ">
              <div class="w-1/2 mr-6 font-size-22">
                <p class="bs-dark-green-color font-size-32 mb-4">Save up to 50% off</p>
                <h2 class="text-6xl font-bold mb-6 text-gray-800">Bengal Vegetable Farm  Organic 100%</h2>
                <p class="mb-8">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vehicula faucibus massa est elit maecenas.</p>
                <nuxt-link to="" class="bs-button text-base">Shop now</nuxt-link>
              </div>
              <div class="w-1/2 flex justify-end">
                <img width="500" src="~/assets/img/hero.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </vue-slick-carousel>
      <div class="container">
        <h3 class="text-4xl mb-6">Search by Categories</h3>
        <div class="flex items-center">
          <div style="height:4px ;width:96px;" class="bs-dark-green-bg"></div>
          <div style="height:2px;" class="bg-gray-400 w-full"></div>
        </div>
        <!-- product carousel -->
        <vue-slick-carousel v-bind="categoryCarouselSettings" class="category-carousel">
          <!-- single carousel -->
            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-1.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-2.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-3.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-4.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-5.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-6.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>

            <div class="bg-gray-200 p-4">
              <div class="h-32 flex justify-center items-center">
                <img src="~/assets/img/product-1.png" alt="">
              </div>
              <h4 class="text-xl text-center">Groceries</h4>
            </div>
            <!-- pervious arrow -->
            <template #prevArrow="arrowOption">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
                </svg>
            </template>
            <!-- next arrow -->
            <template #nextArrow="arrowOption">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"      stroke="currentColor" class="w-6 h-6">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </template>
        </vue-slick-carousel>
      </div>
    </div>
  </div>
</template>

<script>


export default {
    name: "IndexPage",

    data(){
      return{
        categoryCarouselSettings: {
          "slidesToShow": 6,
        }
      }
    }

}
</script>
