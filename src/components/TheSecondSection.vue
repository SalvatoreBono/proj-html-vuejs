<script>
export default {
  components: {},
  data() {
    return {};
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <section class="container pb-5">
    <div class="text-center pb-4">
      <h6 class="fw-bold">YOUR WATCHLIST</h6>
      <h2 class="fw-bold">BEST HITS MOVIES</h2>
    </div>
    <div class="d-flex flex-wrap text-center gap-3">
      <div class="structure">
        <img src="../assets/Gallery-01.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">SEVENTEENTH SUMMER</h4>
        <p class="text-secondary">Commercial, Music Video.</p>
      </div>
      <div class="structure">
        <img src="../assets/Gallery-02.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2">A MESSAGE TO SPACE</h4>
        <p class="text-secondary">Short Film</p>
      </div>
      <div class="structure">
        <img src="../assets/Gallery-03.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2">THE MOST BEAUTIFUL THING</h4>
        <p class="text-secondary">Music Video.</p>
      </div>
      <div class="structure">
        <img src="../assets/Gallery-04.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2">PERMISSION TO SPEAK</h4>
        <p class="text-secondary">Documentary</p>
      </div>
      <div class="structure">
        <img src="../assets/Gallery-05.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2">EXPLORE OUR SPACE</h4>
        <p class="text-secondary">Film noir</p>
      </div>
      <div class="structure">
        <img src="../assets/Gallery-06.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2">FILM PRODUCTION</h4>
        <p class="text-secondary">Blaxploitation</p>
      </div>
    </div>
  </section>
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
</template>

<style lang="scss" scoped>
.structure {
  width: calc(100% / 3 - 1rem);
  padding-bottom: 1rem;
}
img {
  width: 100%;
}
.structure:hover img {
  transform: scale(1.05);
  transition: 0.5s;
}
.bg-counter {
  background-image: url(../assets/Parallax-01.jpg);
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
