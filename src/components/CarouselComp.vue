<template>
  <section class="carousel-section">
    <transition name="fade" mode="in-out">
      <div class="carousel-slide" :key="currentIndex">
        <img :src="slides[currentIndex].src" :alt="slides[currentIndex].caption" />
        <div class="carousel-caption">
          <h2 class="subtitle has-text-white has-text-centered">
            {{ slides[currentIndex].caption }}
          </h2>
        </div>
      </div>
    </transition>
  </section>
</template>

<script>
import Imagem1 from "../assets/carousel/Imagem1.png";
import Imagem2 from "../assets/carousel/Imagem2.png";

export default {
  name: "CarouselComp",
  data() {
    return {
      currentIndex: 0,
      slides: [
        { src: Imagem1, caption: "Bem-vindo ao nosso site!" },
        { src: Imagem2, caption: "Conheça nossos serviços exclusivos" },
      ],
      intervalId: null,
      intervalMs: 10000,
      fadeMs: 800,
    };
  },
  mounted() {
    this.startCarousel();
  },
  beforeUnmount() {
    this.stopCarousel();
  },
  methods: {
    startCarousel() {
      this.intervalId = setInterval(() => {
        this.currentIndex = (this.currentIndex + 1) % this.slides.length;
      }, this.intervalMs);
    },
    stopCarousel() {
      if (this.intervalId) {
        clearInterval(this.intervalId);
        this.intervalId = null;
      }
    },
  },
};
</script>

<style scoped>
.carousel-section {
  position: relative;
  width: 100vw;
  height: 60vh;
  overflow: hidden;
}

.carousel-slide {
  position: absolute;
  inset: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.carousel-caption {
  position: absolute;
  bottom: 1.5rem;
  left: 50%;
  transform: translateX(-50%);
  background: rgba(0, 0, 0, 0.5); /* fundo transparente escuro */
  padding: 0.5rem 1.5rem;
  border-radius: 8px;
}

/* fade */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.8s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.fade-enter-to,
.fade-leave-from {
  opacity: 1;
}
</style>
