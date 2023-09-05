<script>
export default {
  components: {},
  data() {
    return {
      watchlist: [
        {
          img: `Gallery-01.jpg`,
          title: `Seventeenth Summer`,
          overview: `Commercial, Music Video. `,
        },
        {
          img: `Gallery-02.jpg`,

          title: `A Message to Space`,
          overview: `Short Film`,
        },
        {
          img: `Gallery-03.jpg`,

          title: `The most beautiful thing `,
          overview: `Music Video `,
        },
        {
          img: `Gallery-04.jpg`,

          title: `Permission To Speak `,
          overview: `Documentary  `,
        },
        {
          img: `Gallery-05.jpg`,

          title: `Explore our space`,
          overview: `Film noir `,
        },
        {
          img: `Gallery-06.jpg`,

          title: `Film Production `,
          overview: `Blaxploitation  `,
        },
      ],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <!-- START SECOND SECTION -->
  <section class="container pb-5">
    <div class="text-center pb-4">
      <h6 class="fw-bold">YOUR WATCHLIST</h6>
      <h2 class="fw-bold">BEST HITS MOVIES</h2>
    </div>
    <div class="d-flex flex-wrap text-center gap-3">
      <!-- START FOR -->

      <div v-for="singleWatchlist in watchlist" class="structure">
        <div class="animation">
          <img :src="`../src/assets/${singleWatchlist.img}`" alt="" />
        </div>
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">
          {{ singleWatchlist.title }}
        </h4>
        <p class="text-secondary">{{ singleWatchlist.overview }}</p>
      </div>
      <!-- END FOR -->
    </div>
  </section>
  <!-- END SECOND SECTION -->

  <!-- START SECOND BANNER -->
  <section class="pt-5 pb-5">
    <div class="bg-counter d-flex align-items-center">
      <div class="container text-white">
        <div class="d-flex flex-wrap">
          <div class="d-flex flex-column text-center stucture-width-4">
            <div class="fw-bold pb-2 display-4">158</div>
            <div class="text-uppercase fw-bold">satisfield clients</div>
          </div>
          <div class="d-flex flex-column text-center stucture-width-4">
            <div class="fw-bold pb-2 display-4">3+</div>
            <div class="text-uppercase fw-bold">our projects</div>
          </div>
          <div class="d-flex flex-column text-center stucture-width-4">
            <div class="fw-bold pb-2 display-4">1,906</div>
            <div class="text-uppercase fw-bold">cup fo coffee</div>
          </div>
          <div class="d-flex flex-column text-center stucture-width-4">
            <div class="fw-bold pb-2 display-4">2</div>
            <div class="text-uppercase fw-bold">our awards</div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- END SECOND BANNER -->
</template>

<style lang="scss" scoped>
.structure {
  width: calc(100% / 3 - 1rem);
  padding-bottom: 1rem;
}
img {
  width: 100%;
}
.animation {
  overflow: hidden;
}
.structure img {
  transition: 0.5s;
}

.structure:hover img {
  transform: scale(1.05);
}
.bg-counter {
  background-image: url(../assets/Parallax-01.jpg);
  background-attachment: fixed;
  width: 100%;
  height: 250px;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.stucture-width-4 {
  width: calc(100% / 4);
}
</style>
