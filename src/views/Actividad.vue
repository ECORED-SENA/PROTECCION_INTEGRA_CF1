<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
  
    .titulo-principal
      .titulo-principal__numero
        .h3
          i.fas.fa-question-circle
      .h3 Actividad didactica
    
    .row.align-items-center.justify-content-center
        .col-8.col-md-5.col-xl-4.mb-5
            figure
                img(src="@/assets/componentes/img_actividad.svg")
        .col-12.col-md-7
            hr.line-100.bg-orange
            .text-center.p-2
                h2 ¡Pon a prueba tu conocimiento! 
                p.mb-4 La siguiente actividad tiene como propósito validar los conocimientos relacionados con el tema <strong>Estrategia de alertas para la permanencia escolar</strong>.
                a(:href="obtenerLink('/actividad/index.html')" target="_blank" class="styleButton") Iniciar            
            hr.line-100.bg-orange

</template>

<script>
import BannerInterno from '../components/plantilla/BannerInterno'
export default {
  name: 'Actividad',
  components: {
    BannerInterno,
  },
  data: () => ({
    globalData: global,
  }),
}
</script>

<style lang="sass" scoped>
.introduccion
</style>
