<template>
  <q-parallax src="~assets/encontro.jpg" :height="1000">
    <div class="row text-center items-center">
      <div class="col-12 col-md-2"></div>
      <div class="col-12 col-md-6">
        <img alt="Encontro UJ24" src="~assets/unico-logo.png" />
        <q-btn
          label="INSCREVA-SE AGORA"
          style="opacity: 75%"
          size="xl"
          rounded
          color="primary"
        />
      </div>
      <div class="col-12 col-md-2 text-h2 text-center">
        <strong>19, 20 e 21</strong>
        <section class="text-h4">
          <strong>DE OUTUBRO</strong>
        </section>
      </div>
    </div>
  </q-parallax>
  <countdown />
  <q-img src="~/assets/awaken-desktop.gif"/>
</template>

<script>
import Countdown from "src/components/Countdown.vue";
import { defineComponent } from "vue";

export default defineComponent({
  components: { Countdown },
  name: "IndexPage",
  setup() {},
});
</script>
