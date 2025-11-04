<template lang="">
  <nav class="navbar is-fixed-top is-white p-2" role="navigation" aria-label="main navigation">
    <div class="container">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="@/assets/logo.png" height="45" alt="Consultoria em MEI" />
        </a>

        <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item" href="/"> Inicio </a>

          <a class="navbar-item" href="/empresa"> A Empresa </a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link"> Serviços </a>

            <div class="navbar-dropdown">
              <a class="navbar-item"> Serviço 1 </a>
              <a class="navbar-item"> Serviço 2 </a>
              <a class="navbar-item"> Serviço 3 </a>
              <a class="navbar-item"> Serviço 4 </a>
            </div>
          </div>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link"> Parcerias </a>

            <div class="navbar-dropdown">
              <a class="navbar-item" href="/parceiros-especiais"> Parceiros Especiais </a>
              <a class="navbar-item" href="/parceiros"> Parceiros </a>
              <a class="navbar-item" href="/contato"> Quero ser um parceiro </a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <a class="navbar-item" href="https://www.instagram.com/" target="_blank">
            <i class="fab fa-instagram"></i>
          </a>
          <a class="navbar-item" href="https://www.facebook.com/" target="_blank">
            <i class="fab fa-facebook"></i>
          </a>
          <a class="navbar-item" href="https://bit.ly/2vUZIEi" target="_blank">
            <i class="fab fa-whatsapp"></i>
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "NavBar",
};
</script>
<style lang=""></style>
