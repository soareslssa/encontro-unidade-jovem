<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="bg-black text-white text-h2">


        <q-toolbar-title>
          Encontro UJ*24
        </q-toolbar-title>

        <div class="q-gutter-md">
          <q-btn flat label="O QUE É?"/>
          <q-btn flat label="PARA QUEM ?"/>
          <q-btn flat label="INSCRIÇÕES"/>
        </div>
      </q-toolbar>
    </q-header>



    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'


export default defineComponent({
  name: 'MainLayout',

  setup () {

    return {

    }
  }
})
</script>
