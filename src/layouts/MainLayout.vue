<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="bg-black text-white">
        <q-toolbar-avatar class="relative">
          <img src="~/assets/unico-logo.png" width="120" />
        </q-toolbar-avatar>

        <div class="q-gutter-lg col-md-12 text-center">
          <q-btn flat label="O QUE É?" />
          <q-btn flat label="INSCRIÇOES" />
          <q-btn flat label="PARA QUEM ?" />
          <q-btn rounded color="primary" label="INSCRIÇÕES" />
        </div>
      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {
    return {};
  },
});
</script>
