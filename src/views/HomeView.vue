<template>
  <div class="home">
    <section class="section">
      <div class="container">
        <!-- Header -->
        <h1 class="title has-text-centered has-text-weight-bold is-capitalized">Consultoria empresarial para MEI</h1>

        <hr class="my-6" />

        <div class="columns is-vcentered">
          <div class="column">
            <SobreHome />
          </div>

          <div class="is-hidden-mobile is-hidden-tablet-only column is-1"></div>

          <div class="column is-full-mobile is-4-desktop">
            <div class="has-text-centered"><FormIndex /></div>
          </div>
        </div>

        <hr class="my-6" />

        <div class="has-text-centered"><ContatoBar /></div>

        <hr class="my-6" />

        <div class="has-text-centered"><CardsRelacionados /></div>

        <hr class="my-6" />

        <div class="has-text-centered">
          <ParceirosVue />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import SobreHome from "@/components/SobreHome.vue";
import FormIndex from "@/components/FormIndex.vue";
import ContatoBar from "@/components/ContatoBar.vue";
import CardsRelacionados from "@/components/CardsRelacionados.vue";
import ParceirosVue from "@/components/ParceirosVue.vue";

export default {
  components: {
    SobreHome,
    FormIndex,
    ContatoBar,
    CardsRelacionados,
    ParceirosVue,
  },
};
</script>
