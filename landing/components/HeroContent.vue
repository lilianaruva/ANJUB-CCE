<template>
  <div class="pt-24">
    <div
      class="container px-3 mx-auto flex flex-wrap flex-col md:flex-row items-center"
    >
      <!--Left Col-->
      <div
        class="flex flex-col w-full md:w-2/5 justify-center items-start text-center md:text-left"
      >
        <p class="uppercase tracking-loose w-full">Me jubilé, ¿Y ahora qué?</p>
        <h1 class="my-4 text-5xl font-bold leading-tight">
          Asociación Nacional de Jubilados de los Centros de Control Eléctrico
        </h1>
        <p class="leading-normal text-2xl mb-8">
          ANJUB-CCE
        </p>

        <button
          class="mx-auto lg:mx-0 hover:underline bg-white text-gray-800 font-bold rounded-full my-6 py-4 px-8 shadow-lg"
        >
          Subscribe
        </button>
      </div>
      <!--Right Col-->
      <div class="w-full md:w-3/5 py-6 text-center">
        <lottie  :options="lottieOptions" v-on:animCreated="handleAnimation" />
       <!--  <img class="w-full md:w-4/5 z-50" src="~/assets/img/hero.png" alt />  -->
      </div>
    </div>
  </div>
</template>

<script>
import lottie from 'vue-lottie/src/lottie.vue'
import * as animationData from "~/assets/negocios.json";

export default {
  components: {
    lottie,
  },
  data() {
    return {
      anim: null, // for saving the reference to the animation
      lottieOptions: { animationData: animationData.default }
    }
  },
  methods: {
     handleAnimation: function (anim) {
      this.anim = anim;
    }
  },
  name: 'HeroContent'
}
</script>
