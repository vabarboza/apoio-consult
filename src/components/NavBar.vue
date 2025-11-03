<template lang="">
  <nav
    class="navbar is-fixed-top is-white"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="container">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="@/assets/logo.png" height="45" alt="Consultoria em MEI" />
        </a>

        <a
          role="button"
          class="navbar-burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item" href="/"> Inicio </a>

          <a class="navbar-item"> Documentation </a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link"> More </a>

            <div class="navbar-dropdown">
              <a class="navbar-item"> About </a>
              <a class="navbar-item is-selected"> Jobs </a>
              <a class="navbar-item"> Contact </a>
              <hr class="navbar-divider" />
              <a class="navbar-item"> Report an issue </a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <a
            class="navbar-item"
            href="https://www.instagram.com/"
            target="_blank"
          >
            <i class="fab fa-instagram"></i>
          </a>
          <a
            class="navbar-item"
            href="https://www.facebook.com/"
            target="_blank"
          >
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
