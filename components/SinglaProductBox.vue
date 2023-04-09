<template>
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
  <h4 class="text-xl text-center">Product Name - {{ product }}</h4>
  <p><span class="font-medium bs-dark-orange-color">$200.00</span> <del class="text-gray-400">$300.00</del></p>
</div>
</template>
<script>
export default {
  name: 'SingleProductBox',
  props: ['product']

}
</script>
<style scoped>

</style>


