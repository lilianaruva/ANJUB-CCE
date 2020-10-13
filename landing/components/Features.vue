<template>
  <section class="bg-white border-b py-8">
    <div class="container max-w-5xl mx-auto m-8">
      <h1
        class="w-full my-2 text-5xl font-bold leading-tight text-center text-gray-800"
      >
        Conócenos
      </h1>
      <div class="w-full mb-4">
        <div
          class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
        ></div>
      </div>
      <feature-right
        headline="Quienes somos"
        content="Asociación Civil sin fines de lucro, integrada por ex-trabajadores del CENACE OPD, jubilados de sus diversos centros en el país."
      >
        <img src="~assets/img/travel-booking.svg?inline" alt slot="svg" />
      </feature-right>
      <feature-left
        headline="Misión"
        content="Promover la unidad entre los Asociados y la preservación de los derechos adquiridos como trabajadores jubilados del CENACE OPD, implementando acciones que promuevan su bienestar social y calidad de vida, en un ambiente de convivencia armónica y respetuosa, con asesoría y acompañamiento especializado."
      >
        <img src="~assets/img/connected-world.svg?inline" alt slot="svg" />
      </feature-left>
    </div>
  </section>
</template>

<script>
import FeatureRight from '@/components/FeatureRight'
import FeatureLeft from '@/components/FeatureLeft'

export default {
  name: 'Features',
  components: {
    'feature-right': FeatureRight,
    'feature-left': FeatureLeft
  }
}
</script>
