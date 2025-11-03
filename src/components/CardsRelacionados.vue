<template>
  <div class="section">
    <!-- Título -->
    <div class="mb-5">
      <p class="title is-4 has-text-weight-bold">Páginas Relacionadas</p>
    </div>

    <!-- Grid de cards -->
    <div class="columns is-multiline">
      <!-- Card 1 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner1.png"
              alt="Banner 1"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>

      <!-- Card 2 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner2.png"
              alt="Banner 2"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>

      <!-- Card 3 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner3.png"
              alt="Banner 3"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>

      <!-- Card 4 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner4.png"
              alt="Banner 4"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>

      <!-- Card 5 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner5.png"
              alt="Banner 5"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>

      <!-- Card 6 -->
      <div class="column is-full-mobile is-half-tablet is-one-third-desktop">
        <div class="box p-0">
          <a href="#!">
            <img
              src="../assets/cards/banner6.png"
              alt="Banner 6"
              class="image is-fullwidth"
            />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardsRelacionados",
};
</script>

<style scoped>
/* Remover padding interno da box para a imagem ocupar todo o espaço */
.box.p-0 {
  padding: 0;
}

/* Opcional: borda arredondada na imagem */
img.image {
  border-radius: 6px;
}

/* Se quiser efeito de hover tipo zoom, pode adicionar */
.box:hover img {
  transform: scale(1.05);
  transition: transform 0.3s ease-in-out;
}
</style>
