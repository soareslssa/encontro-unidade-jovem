<template>
  <q-parallax src="~assets/encontro.jpg" :height="1000">
    <img alt="Encontro UJ24" src="~assets/unico-logo.png" />
  </q-parallax>
  <countdown />
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
