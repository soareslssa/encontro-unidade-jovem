<template>
  <q-parallax src="~assets/encontro.jpg" :height="1000">
    <img alt="Encontro UJ24" src="~assets/unico-logo.png" />
  </q-parallax>
  <div class="bg-black row text-center justify-center text-h4 q-pa-md">
    <div class="col-12 col-md-auto items-start">
      <img src="~/assets/unico-logo.png" width="150"/>
    </div>
    <div class="col-12 col-md-1">
      {{ days % 365}}
      <section>DIAS</section>
    </div>
    <div class="col-12 col-md-1">
      {{ hours % 24 }}
      <section>HORAS</section>
    </div>
    <div class="col-12 col-md-1">
      {{ minutes % 60}}
      <section>MIN</section>
    </div>
    <div class="col-12 col-md-1">
      {{ seconds % 60}}
      <section>SEC</section>
    </div>
    <div class="col-12 col-md-auto ">
      <q-btn label="INSCREVA-SE AGORA" rounded color="primary"/>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    let days = ref(0);
    let hours = ref(0);
    let minutes = ref(0);
    let seconds = ref(0);

    const dataEncontro = new Date("20 October 2024");
    setInterval(() => {
      const currentDate = new Date();
      const lunchTime = dataEncontro - currentDate;

      seconds.value = parseInt(lunchTime / 1000);
      minutes.value = parseInt(seconds.value / 60);
      hours.value = parseInt(minutes.value / 60);
      days.value = parseInt(hours.value / 24);
    }, 1000);

    return {
      days,
      hours,
      minutes,
      seconds
    };
  },
});
</script>
