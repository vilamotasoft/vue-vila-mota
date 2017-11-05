<template>
  <div class="home">
    <q-card>
      <q-card-title>
        Nosso Escritório
      </q-card-title>
      <q-card-separator />
      <q-card-main>
        <p>
          Advogadas Caroline Perez e Caroline Velho, montaram um escritório de advocacia que prima por serviços jurídicos de alta qualidade, 
          atuando de forma criteriosa na defesa de seus clientes. Na busca de não somente soluções momentâneas, 
          mas, sobretudo, a resolução plena dos problemas e desafios propostos. Através da assessoria jurídica da 
          as Advogadas Caroline Perez e Caroline Velho a pessoalidade no atendimento, bem como a atenção a cada caso, são uma constante. 
          O envolvimento nas causas de seus clientes e a singularidade e dedicação empregadas em cada caso.
        </p>
      </q-card-main>
      <q-card-separator />
      <q-card-media>
        <q-gallery infinite autoplay dots fullscreen :src="slider"></q-gallery>
      </q-card-media>
    </q-card>
  </div>
</template>

<script>
import { QCard, QCardMedia, QCardTitle, QCardSeparator, QCardMain, QGallery } from 'quasar'
export default {
  name: 'home',
  data () {
    return {
      slider: [
        'statics/escritorio1.jpg',
        'statics/escritorio2.jpg'
      ]
    }
  },
  components: {
    QCard,
    QCardMedia,
    QCardTitle,
    QCardSeparator,
    QCardMain,
    QGallery
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
@import '~variables'

</style>
