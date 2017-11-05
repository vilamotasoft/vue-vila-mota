<template>
  <!-- Don't drop "q-app" class -->
  <div id="q-app">
    <!-- <header></header> -->
    <q-layout ref="layout" >
      <!-- Header -->
      <q-toolbar slot="header" class="bg-negative">
        <q-btn flat @click="$refs.layout.toggleLeft()">
          <q-icon name="menu" />
        </q-btn>
        <q-toolbar-title>
          Advocacia
          <span slot="subtitle">Procure seu Direito</span>
        </q-toolbar-title>
      </q-toolbar>
      <!-- Left Side Panel -->
      <div slot="left">
        <q-list no-border link inset-separator>
          <q-list-header>Menu</q-list-header>
          <q-side-link item to="/home">
            <q-item-side icon="store" />
            <q-item-main label="Nosso Escritório" />
          </q-side-link>
          <q-side-link item to="/gavel">
            <q-item-side icon="gavel" />
            <q-item-main label="Atuação" />
          </q-side-link>
          <q-side-link item to="/people">
            <q-item-side icon="people" />
            <q-item-main label="Advogadas" />
          </q-side-link>
          <q-side-link item to="/contacts">
            <q-item-side icon="contacts" />
            <q-item-main label="Contatos" />
          </q-side-link>
          <q-side-link item to="/input">
            <q-item-side icon="input" />
            <q-item-main label="Acesso Restrito" />
          </q-side-link>
        </q-list>
      </div>   
      <!-- sub-routes get injected here: -->
      <router-view />
      <!-- Footer -->
      <q-toolbar slot="footer" class="bg-negative">
        <q-toolbar-title>
          <div class="vm-footer">
            Vila Mota Software
          </div>
        </q-toolbar-title>
      </q-toolbar>
    </q-layout>
  </div>
</template>

<script>
/*
 * Root component
 */
import { QLayout, QToolbar, QToolbarTitle, QBtn, QIcon, QList, QListHeader, QSideLink, QItemSide, QItemMain } from 'quasar'
export default {
  components: {
    QLayout,
    QToolbar,
    QToolbarTitle,
    QBtn,
    QIcon,
    QList,
    QListHeader,
    QSideLink,
    QItemSide,
    QItemMain
  }
}
</script>

<style lang="stylus">
@import '~variables'

.vm-footer
  text-align center

</style>
