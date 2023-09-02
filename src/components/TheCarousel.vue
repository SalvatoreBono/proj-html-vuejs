<script>
export default {
  components: {},
  data() {
    return {
      Carousel: [
        {
          img: `67359-Root-Film-HD-Wallpaper.jpg`,
          smallTitle: `cinemato studio`,
          title: `action and inspire people`,
        },
        {
          img: `chainsaw-man-anime-opening-hd-wallpaper-uhdpaper.com-766@1@i.jpg`,
          smallTitle: `cinemato director`,
          title: `Dancing with of the stars`,
        },
      ],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <div id="carouselExampleFade" class="carousel slide carousel-fade">
    <div class="carousel-inner">
      <div v-for="SingleCarousel in Carousel" class="carousel-item active">
        <img
          :src="`src/assets/${SingleCarousel.img}`"
          class="d-block w-100"
          alt="..."
        />
        <div class="card-title text-uppercase col-4 custom-description">
          <h5 class="fw-bold">{{ SingleCarousel.smallTitle }}</h5>
          <h1 class="display-3 fw-bold">{{ SingleCarousel.title }}</h1>
          <button
            type="button"
            class="rounded-0 fw-bold btn btn-light pe-4 ps-4 pt-2 pb-2 mt-4"
          >
            READ MORE
          </button>
        </div>
      </div>
    </div>
    <div class="btn-carousel">
      <button
        type="button"
        class="btn btn-custom rounded-0 ms-3"
        data-bs-target="#carouselExampleFade"
        data-bs-slide="prev"
      >
        <i class="fa-solid fa-chevron-left"></i>
      </button>
      <button
        type="button"
        class="btn btn-custom rounded-0 me-3"
        data-bs-target="#carouselExampleFade"
        data-bs-slide="next"
      >
        <i class="fa-solid fa-chevron-right"></i>
      </button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
img {
  height: 800px;
}
.btn-carousel {
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  display: flex;
  justify-content: space-between;
  z-index: 1;
}
.btn-custom {
  background-color: rgba(0, 0, 0, 0.3);
  color: white;
  font-size: 20px;
  opacity: 0;
}
.custom-description {
  position: absolute;
  top: 40%;
  left: 15%;
  color: white;
}
.carousel:hover .btn-custom {
  opacity: 1;
}
.btn-custom:hover {
  background-color: rgba(0, 0, 0, 0.8);
  color: white;
}
.btn:active {
  color: white !important;
  background-color: rgba(0, 0, 0, 0.8) !important;
}
</style>
