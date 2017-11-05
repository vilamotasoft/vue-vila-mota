<template>
  <div class="people">
    <q-card>
      <q-card-title>
        ADVOGADAS
      </q-card-title>
      <q-card-separator />
      <q-card-main>
        <p>Caroline Perez Pereira</p>
        <p>OAB/RS 88.357</p>
      </q-card-main>
      <q-card-separator />
      <q-card-main>
        <p>Caroline Moreira Velho Etges</p>
        <p>OAB/RS 83.890</p>
      </q-card-main>
    </q-card>
  </div>
</template>

<script>
import { QCard, QCardTitle, QCardSeparator, QCardMain } from 'quasar'
export default {
  name: 'people',
  components: {
    QCard,
    QCardTitle,
    QCardSeparator,
    QCardMain
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus">
@import '~variables'
</style>
