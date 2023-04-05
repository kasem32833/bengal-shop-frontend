<template>
  <div>

    <!-- <vue-slick-carousel :arrows="true" :dots="true">
      <div>1</div>
      <div>2</div>
      <div>3</div>
      <div>4</div>
    </vue-slick-carousel> -->

<!-- Hero slide carousel -->
    <div class="p-8 relative">
      <vue-slick-carousel :arrows="false" :dots="true" class="hero-slide">
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


      <div class="container pt-20">
         <!-- categories section -->
        <h3 class="text-4xl mb-6">Search by Categories</h3>
        <!-- line design -->
        <div class="flex items-center mb-10">
          <div style="height:4px ;width:96px;" class="bs-dark-green-bg"></div>
          <div style="height:2px;" class="bg-gray-400 w-full"></div>
        </div>
        <!-- product carousel -->
        <vue-slick-carousel v-bind="categoryCarouselSettings" class="category-carousel mb-10">

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
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 text-white">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 19.5L8.25 12l7.5-7.5" />
                </svg>
            </template>
            <!-- next arrow -->
            <template #nextArrow="arrowOption">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"      stroke="currentColor" class="w-6 h-6 text-white">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </template>
        </vue-slick-carousel>
        <!-- Promo section -->
        <div class="flex -mx-6 mb-14">
          <div class="px-6 w-1/2">
            <div class="promo-bg-1 bg-gray-200 p-20 rounded bg-cover bg-center">
              <div class="w-2/3">
                <p class="text-2xl bs-dark-orange-color">Buy 1 Get 1</p>
                <h1 class="font-bold text-3xl text-gary-800 my-6">Fresh Vegetable Collection</h1>
                <nuxt-link to="/" class="promo-button ">Order Now</nuxt-link>
              </div>
            </div>
          </div>
          <div class="px-6 w-1/2">
            <div class="promo-bg-2 bg-gray-200 p-20 rounded bg-cover bg-center">
              <div class="w-2/3">
                <p class="text-2xl bs-dark-orange-color">Buy 1 Get 1</p>
                <h1 class="font-bold text-3xl text-gary-800 my-6">Fresh Vegetable Collection</h1>
                <nuxt-link to="/" class="promo-button ">Order Now</nuxt-link>
              </div>
            </div>
          </div>
        </div>
        <!-- deals of the weak section -->
        <h3 class="text-4xl mb-6">Deals of the Week</h3>
        <!-- line design -->
        <div class="flex items-center mb-10">
          <div style="height:4px ;width:96px;" class="bs-dark-green-bg"></div>
          <div style="height:2px;" class="bg-gray-400 w-full"></div>
        </div>
        <!-- deals carousel -->
      <vue-slick-carousel v-bind="dealsCarouselSetting" class="category-carousel mb-16 text-center">

        <div class="single-bs-product">
          <div class=" h-80 relative  mb-6 ">
            <!-- bg image -->
            <div class="bg-gray-50 flex justify-center items-center p-4 w-full h-full ">
              <img src="~/assets/img/deal-1.png" alt="">
            </div>
            <!-- hover design -->
            <div class=" product-image-hover bg-black opacity-60 absolute flex justify-center items-center left-0 top-0 w-full h-full">
              <div class=" flex flex-col space-y-4 justify-center items-center">
                <div class="flex space-x-2 relative ">
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold">+</button>
                  <span class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">1</span>
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">-</button>
                </div>
                <button to="" class="bs-button">Add to cart</button>
                <nuxt-link to="/" class="flex w-full  justify-center items-center absolute bottom-0 left-0 bg-red-500 text-white">
                  Details
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
                  </svg>
                </nuxt-link>
              </div>
            </div>
          </div>
          <h4 class="text-xl text-center">Product Name</h4>
          <p><span class="font-medium bs-dark-orange-color">$200.00</span> <del class="text-gray-400">$300.00</del></p>
        </div>

        <div class="single-bs-product">
          <div class="h-80 relative  mb-6 ">
            <div class="bg-gray-50 flex justify-center items-center p-4 w-full h-full">
              <img src="~/assets/img/deal-1.png" alt="">
            </div>
            <div class=" product-hover absolute flex justify-center items-center left-0 top-0 w-full h-full ">
              <div class="flex-col space-y-4 justify-center items-center hidden group-hover:flex ">
                <div class="flex space-x-2 relative">
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold">+</button>
                  <span class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">1</span>
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">-</button>
                </div>
                <button to="" class="bs-button">Add to cart</button>
                <nuxt-link to="/" class="flex w-full  justify-center items-center absolute bottom-0 left-0 bg-red-500 text-white">
                  Details
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
                  </svg>
                </nuxt-link>
              </div>
            </div>
          </div>
          <h4 class="text-xl text-center">Product Name</h4>
          <p><span class="font-medium bs-dark-orange-color">$200.00</span> <del class="text-gray-400">$300.00</del></p>
        </div>

        <div class="single-bs-product">
          <div class=" h-80  relative  mb-6 ">
            <div class="bg-gray-50 flex justify-center items-center p-4 w-full h-full">
              <img src="~/assets/img/deal-1.png" alt="">
            </div>
            <div class=" product-hover absolute flex justify-center items-center left-0 top-0 w-full h-full  ">
              <div class="flex-col space-y-4 justify-center items-center hidden group-hover:flex ">
                <div class="flex space-x-2 relative">
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold">+</button>
                  <span class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">1</span>
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">-</button>
                </div>
                <button to="" class="bs-button">Add to cart</button>
                <nuxt-link to="/" class="flex w-full  justify-center items-center absolute bottom-0 left-0 bg-red-500 text-white">
                  Details
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
                  </svg>
                </nuxt-link>
              </div>
            </div>
          </div>
          <h4 class="text-xl text-center">Product Name</h4>
          <p><span class="font-medium bs-dark-orange-color">$200.00</span> <del class="text-gray-400">$300.00</del></p>
        </div>
        <div class="single-bs-product">
          <div class=" h-80 relative  mb-6 ">
            <div class="bg-gray-50 flex justify-center items-center p-4 w-full h-full">
              <img src="~/assets/img/deal-1.png" alt="">
            </div>
            <div class=" product-hover absolute flex justify-center items-center left-0 top-0 w-full h-full  ">
              <div class="flex-col space-y-4 justify-center items-center hidden group-hover:flex ">
                <div class="flex space-x-2 relative ">
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold">+</button>
                  <span class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">1</span>
                  <button class="w-8 h-8  border borderwhite rounded-full flex justify-center items-center text-2xl font-bold ">-</button>
                </div>
                <button to="" class="bs-button">Add to cart</button>
                <nuxt-link to="/" class="flex w-full  justify-center items-center absolute bottom-0 left-0 bg-red-500 text-white">
                  Details
                  <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
                  </svg>
                </nuxt-link>
              </div>
            </div>
          </div>
          <h4 class="text-xl text-center">Product Name</h4>
          <p><span class="font-medium bs-dark-orange-color">$200.00</span> <del class="text-gray-400">$300.00</del></p>
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

        <!-- Popular Brands -->
        <h3 class="text-4xl mb-6">Popular Barnds</h3>
        <!-- line design -->
        <div class="flex items-center mb-10">
          <div style="height:4px ;width:96px;" class="bs-dark-green-bg"></div>
          <div style="height:2px;" class="bg-gray-400 w-full"></div>
        </div>
      </vue-slick-carousel>
        <!-- Featured section -->
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
        },
        dealsCarouselSetting: {
          "slidesToShow": 4,
        }

      }
    }

}
</script>
