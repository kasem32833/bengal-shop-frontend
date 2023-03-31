<template>
  <div>
    <div class="container">
      <div class="flex -mx-4 mb-10">
        <div class=" w-1/4 flex px-4 items-center">
          <div class="min-w-max mr-4">
            <img width="80" src="~/assets/img/support.png" alt="">
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">24 Customer Support</h3>
            Contact us 24 hours
          </div>
        </div>

        <div class=" w-1/4 flex px-4 items-center">
          <div class="min-w-max mr-4">
            <img width="80" src="~/assets/img/authentic-product.png" alt="">
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">Authentic Products</h3>
            Contact us 24 hours
          </div>
        </div>

        <div class=" w-1/4 flex px-4 items-center">
          <div class="min-w-max mr-4">
            <img width="80" src="~/assets/img/secure-payment.png" alt="">
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">Secure Payment</h3>
            Contact us 24 hours
          </div>
        </div>

        <div class=" w-1/4 flex px-4 items-center">
          <div class="min-w-max mr-4">
            <img width="80" src="~/assets/img/discount.png" alt="">
          </div>
          <div class="w-full">
            <h3 class="text-xl font-medium mb-2">Best Prices & Offers</h3>
            Contact us 24 hours
          </div>
        </div>
      </div>
    </div>
    <div class="bg-gray-200 py-20">
      <div class="container">
        <div class="flex">
          <div class="w-3/5 pr-10">
            <Logo/>

            <p class="my-8">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla diam ornare nam est gravida. Netus viverra rhoncus sit magna sapien ac eget parturient id. Est luctus dapibus quam aliquam in nisl turpis. Elit et dictum lacus morbi nec accumsan a in.</p>

            <div class="flex mr-4">
              <a href="" target="blank"><img src="~/assets/img/play-store.png" alt=""></a>
              <a href="" target="blank"><img src="~/assets/img/app-store.png" alt=""></a>
            </div>
          </div>
          <div class="w-1/5 pl-6">
            <h3 class="text-2xl mb-6">About Us</h3>
            <ul class="leading-loose">
              <li><nuxt-link to="">About bengal shop</nuxt-link></li>
              <li><nuxt-link to="">Contact</nuxt-link></li>
              <li><nuxt-link to="">Career</nuxt-link></li>
              <li><nuxt-link to="">Terms and condition</nuxt-link></li>
              <li><nuxt-link to="">Categories</nuxt-link></li>
            </ul>
          </div>
          <div class="w-1/5 pl-6">
            <h3 class="text-2xl mb-6">Info</h3>
            <ul class="leading-loose">
              <li><nuxt-link to="">information</nuxt-link></li>
              <li><nuxt-link to="">Shipping</nuxt-link></li>
              <li><nuxt-link to="">Payment</nuxt-link></li>
              <li><nuxt-link to="">Return</nuxt-link></li>
              <li><nuxt-link to="">Blog</nuxt-link></li>
            </ul>
          </div>
        </div>
        <!-- copyrignt section -->
        <div class="flex items-center pt-20">
          <div class="w-1/3">social links</div>
          <div class="w-1/3 text-xs">@2023 Copyright All Right Reserved by Bengal Shop</div>
          <div class="w-1/3"><img src="~/assets/img/payment-gateway.png" alt=""></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>

</style>
