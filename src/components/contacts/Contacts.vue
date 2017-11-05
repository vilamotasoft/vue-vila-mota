<template>
  <div class="contacts">
    <q-card>
      <q-card-title>
        CONTATO
      </q-card-title>
      <q-card-separator />
      <q-card-main>
        <p>(51) 3372-7529</p>
        <p>contato@perezevelho.adv.br</p>
      </q-card-main>
    </q-card>
    <q-card>
      <q-card-title>
        ENDEREÇO
      </q-card-title>
      <q-card-separator />
      <q-card-main>
        <p>Rua Barão do Amazonas, 1866/208</p>
        <p>Partenon</p>
        <p>Porto Alegre/RS</p>
        <p>90670-002</p>
      </q-card-main>
      <q-card-media>
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3453.19929207212!2d-51.19394198467498!3d-30.059821438952916!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9519780fa67a82e5%3A0xd617d7550033e0e5!2sR.+Bar%C3%A3o+do+Amazonas%2C+1866+-+Partenon%2C+Porto+Alegre+-+RS%2C+90670-002!5e0!3m2!1spt-BR!2sbr!4v1509919184234" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
      </q-card-media>
    </q-card>
  </div>
</template>

<script>
import { QCard, QCardTitle, QCardSeparator, QCardMain, QCardMedia } from 'quasar'
export default {
  name: 'contacts',
  components: {
    QCard,
    QCardTitle,
    QCardSeparator,
    QCardMain,
    QCardMedia
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
@import '~variables'
</style>
