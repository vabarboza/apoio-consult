<template>
  <footer class="footer has-background-link-dark pt-6">
    <div class="container">
      <!-- Seção superior -->
      <div class="columns is-multiline">
        <!-- Sobre a empresa -->
        <div class="column is-full-mobile is-5-desktop">
          <h6 class="title is-6 has-text-weight-bold has-text-white mb-4 has-text-left-desktop">
            APOIO – CONSULTORIA PARA MICROEMPREENDEDORES
          </h6>
          <p class="is-size-7 has-text-white has-text-left-desktop">
            A APOIO é uma consultoria especializada em oferecer suporte e
            consultoria personalizada para microempreendedores. Com uma equipe
            de consultores experientes, fornecemos orientação abrangente em
            áreas como planejamento de negócios, estratégias de marketing,
            gestão financeira e organização operacional. Nosso objetivo é
            capacitar os microempreendedores, oferecendo conhecimentos e
            soluções práticas para impulsionar seus negócios e alcançar o
            sucesso desejado.
          </p>
        </div>

        <!-- Links úteis -->
        <div class="column is-full-mobile is-3-desktop">
          <h6 class="title is-6 has-text-weight-bold has-text-white mb-4">Links Úteis</h6>
          <p><a class="has-text-white" href="/contato">Torne-se um parceiro</a></p>
          <p><a class="has-text-white" href="#!">Link de acesso</a></p>
          <p><a class="has-text-white" href="#!">Link de acesso</a></p>
        </div>

        <!-- Contato -->
        <div class="column is-full-mobile is-4-desktop has-text-right-desktop">
          <h6 class="title is-6 has-text-weight-bold has-text-white mb-4 ">Contato</h6>
          <p class="has-text-white"><i class="fas fa-home mr-2"></i> Endereço</p>
          <p class="has-text-white"><i class="fas fa-envelope mr-2"></i> email@gmail.com</p>
          <p class="has-text-white"><i class="fas fa-phone mr-2"></i> (99) 99999-9999</p>
        </div>
      </div>

      <hr class="has-background-white" />

      <!-- Seção inferior -->
      <div class="columns is-vcentered is-multiline">
        <!-- Copyright -->
        <div class="column is-full-mobile is-7-desktop">
          <p class="is-size-7 has-text-centered-mobile has-text-left-desktop has-text-white">
            © {{ anoAtual }} Copyright:
            <a class="has-text-white" href="/">
              <strong> www.apoio.com.br</strong>
            </a>
          </p>
        </div>

        <!-- Redes sociais -->
        <div class="column is-full-mobile is-5-desktop ">
          <div class="has-text-centered-mobile has-text-right-desktop">
            <a class="button is-small is-white is-rounded mx-1" href="#"><i class="fab fa-facebook-f has-text-black"></i></a>
            <a class="button is-small is-white is-rounded mx-1" href="#"><i class="fab fa-instagram has-text-black"></i></a>
            <a class="button is-small is-white is-rounded mx-1" href="#"><i class="fab fa-whatsapp has-text-black"></i></a>
            <a class="button is-small is-white is-rounded mx-1" href="#"><i class="fab fa-linkedin-in has-text-black"></i></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComp",
  data() {
    return {
      anoAtual: new Date().getFullYear(),
    };
  },
};
</script>

<style scoped>
.mx-1 {
  margin-left: 0.25rem;
  margin-right: 0.25rem;
}

.mr-2 {
  margin-right: 0.5rem;
}

/* Hover nas redes sociais */
.button.is-white:hover {
  background-color: #00d1b2;
  color: white;
}
</style>
