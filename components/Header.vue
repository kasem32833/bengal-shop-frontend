<template>
  <div>
    <div class="container">
      <div class="flex justify-between items-center py-6">
        <Logo/>
        <div class="w-96">
          <div class="border border-gray-100 rounded-full p-1 flex items-center ">
            <div class="min-w-max px-3">
              <img src="~/assets/img/search.png" alt="">
            </div>
            <input class="w-full px-3 py-1 focus:outline-none" type="search" placeholder="serach here...">
            <button class="bs-button-bg px-6 py-2 rounded-full text-white" type="submit">search</button>
          </div>
        </div>
        <div class="min-w-max flex items-center space-x-2">
          <nuxt-link to="/"><span class="bs-icon-box rounded-full flex justify-center items-center hover:bg-gray-200 "><img src="~/assets/img/heart.png" alt=""></span></nuxt-link>
          <nuxt-link to="/" class="relative"><span class="bs-icon-box rounded-full flex justify-center items-center hover:bg-gray-200 "><img src="~/assets/img/shopping.png" alt=""></span
            ><span class="absolute bg-red-500 w-4 h-4 top-0 right-0 rounded-full flex justify-center items-center text-sm text-white
            ">0</span></nuxt-link>
          <nuxt-link to="/" class="flex items-center"><span class="bs-icon-box rounded-full flex justify-center items-center hover:bg-gray-200 "><img src="~/assets/img/user.png" alt=""></span><span>Account</span></nuxt-link>
        </div>
      </div>


      <div v-click-outside="menuClose"  class="flex items-center">
        <div class="w-96 relative">
          <div @click.prevent="menuClick" class="flex items-center bs-dark-green-bg rounded-full px-4 py-2 cursor-pointer ">
            <div class="min-w-max">
              <img src="~/assets/img/menu-right.png" alt="">
            </div>
            <div class="w-full text-center px-6 text-white relative z-20 text-lg">All categories</div>
            <div class="min-w-max">
              <img src="~/assets/img/chevron-down.png" alt="">
            </div>
          </div>
          <!-- Categorie slide menu -->
          <div v-bind:class="allCategoryMenu ? 'flex visible'  : 'hidden invisible' " class="   absolute bs-dark-green-bg z-10 w-full -mt-4  flex-col space-y-3 rounded-b-2xl">
            <ul class="py-4 text-center">
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Vegetables</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Groceries</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
              <li><nuxt-link to="" class="py-2 px-4 block text-white hover:text-black">Fruites</nuxt-link></li>
            </ul>
          </div>
        </div>

        <div class="w-full">
          <ul>
            <li class="flex justify-center">
              <nuxt-link to="#" class="p-4">Home</nuxt-link>
              <nuxt-link to="#" class="p-4">Shop</nuxt-link>
              <nuxt-link to="#" class="p-4">Categories</nuxt-link>
              <nuxt-link to="#" class="p-4">Offers</nuxt-link>
              <nuxt-link to="#" class="p-4">Contact</nuxt-link>
              <nuxt-link to="#" class="p-4">FAQs</nuxt-link>
            </li>
          </ul>
        </div>
        <nuxt-link to="/" class="min-w-max flex">
          <img src="~/assets/img/percentage.png" alt="" class="mr-3"> Special Offers!
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",

  data(){
    return{
      allCategoryMenu: false,
    }
  },
  methods:{
    menuClick (){
      this.allCategoryMenu = !this.allCategoryMenu;
    },
    menuClose(){


      this.allCategoryMenu = false;
    }
  }

}
</script>

<style scoped>

</style>
