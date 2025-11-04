<template>
  <div class="columns is-vcentered is-multiline mt-3 mb-3">
    <!-- Texto -->
    <div class="column is-full-mobile is-7-desktop">
      <p class="title is-4 has-text-weight-bold">Encontrou o que procurava?</p>
      <h6 class="subtitle is-6">Faça seu orçamento grátis agora mesmo!</h6>
    </div>

    <!-- Espaço opcional entre colunas -->
    <div class="is-hidden-mobile column is-1"></div>

    <!-- Botão -->
    <div class="column is-full-mobile is-4-desktop">
      <button class="button is-dark is-rounded is-fullwidth" @click="irParaContato">ENTRAR EM CONTATO</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContatoBar",
  methods: {
    irParaContato() {
      // Redireciona para a página de contato
      window.location.href = "/contato";
    },
  },
};
</script>

<style scoped>
/* Ajustes opcionais de margin */
.mt-3 {
  margin-top: 1rem;
}
.mb-3 {
  margin-bottom: 1rem;
}
</style>
