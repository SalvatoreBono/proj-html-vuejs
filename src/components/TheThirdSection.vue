<script>
export default {
  components: {},
  data() {
    return {
      team: [
        {
          img: `Team-01.jpg`,
          title: `Fabricio guerra`,
          overview: `Main Director`,
        },
        {
          img: `Team-02.jpg`,
          title: `umberto pagoda`,
          overview: `Main Writer`,
        },
        {
          img: `Team-03.jpg`,
          title: `gloria riccasso`,
          overview: `Main Producer`,
        },
        {
          img: `Team-04.jpg`,
          title: `Lio napoin `,
          overview: `Cameraman`,
        },
      ],
      carousel: [
        {
          img: `01.jpg`,
        },
        {
          img: `02.jpg`,
        },
        {
          img: `03.jpg`,
        },
      ],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <!-- START THIRD SECTION -->
  <section class="container pt-5 pb-5">
    <div class="text-center pb-4">
      <h6 class="fw-bold text-uppercase">the pericuros</h6>
      <h2 class="fw-bold text-uppercase">Meet the team</h2>
    </div>

    <div class="d-flex flex-wrap text-center gap-4">
      <!-- START FOR -->
      <div v-for="SingleTeam in team" class="stucture-width-4">
        <div class="animation">
          <img :src="`src/assets/${SingleTeam.img}`" alt="" />
        </div>
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">{{ SingleTeam.title }}</h4>
        <p class="text-secondary">{{ SingleTeam.overview }}</p>
      </div>
      <!-- END FOR -->
    </div>
  </section>
  <!-- END THIRD SECTION -->

  <!-- START BANNER -->
  <section class="bg-about-us mb-5 d-flex align-items-center">
    <div
      class="container justify-content-center align-items-center text-center d-flex flex-column text-white"
    >
      <div class="col-6">
        <img
          style="width: 50px"
          class="mb-5"
          src="../assets/image (20).svg"
          alt=""
        />
        <!-- START CAROUSEL -->

        <div id="carouselExampleCaptions" class="carousel slide">
          <div style="top: 170px" class="carousel-indicators">
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              data-bs-slide-to="0"
              style="width: 10px; height: 10px; border-radius: 50%"
              class="active"
              aria-current="true"
              aria-label="Slide 1"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              style="width: 10px; height: 10px; border-radius: 50%"
              class="me-2 ms-2"
              data-bs-slide-to="1"
              aria-label="Slide 2"
            ></button>
            <button
              type="button"
              data-bs-target="#carouselExampleCaptions"
              style="width: 10px; height: 10px; border-radius: 50%"
              data-bs-slide-to="2"
              aria-label="Slide 3"
            ></button>
          </div>
          <div class="carousel-inner">
            <!-- START FOR -->

            <div
              v-for="singleCarousel in carousel"
              class="carousel-item active"
            >
              <p>
                Curabitur bindum ex ut sapien blandit viverra. Nunc lobortis mi
                dui, id Etiam tempor sit amet metus in bibendum. Nunc eros
                risus, pellentesque a augue pellentesque fringilla eget mi eu
                mollis. commodo.
              </p>
              <div class="d-flex justify-content-center">
                <div class="me-3">
                  <img
                    class="rounded-circle"
                    :src="`src/assets/${singleCarousel.img}`"
                    alt=""
                  />
                </div>
                <div class="d-flex flex-column text-start">
                  <div class="text-uppercase fw-bold">John doe</div>
                  <div class="small">Designer</div>
                </div>
              </div>
            </div>
            <!-- END FOR -->
          </div>
        </div>
        <!-- END CAROUSEL -->
      </div>
    </div>
  </section>
  <!-- END THIRD SECTION -->
</template>

<style lang="scss" scoped>
.stucture-width-4 {
  width: calc(100% / 4 - 2rem);
}
.stucture-width-4 img {
  transition: 0.5s;
}
.animation {
  overflow: hidden;
}
.structure img {
  transition: 0.5s;
}

.stucture-width-4:hover img {
  transform: scale(1.05);
}
.bg-about-us {
  background-image: url(../assets/Parallax-02.jpg);
  background-attachment: fixed;
  width: 100%;
  height: 600px;
  background-size: cover;
  background-repeat: no-repeat;
}
img {
  width: 100%;
}
i {
  padding-left: 0.5rem;
  cursor: pointer;
}
.bg-about-us img {
  width: 60px;
}

button {
  width: 50px;
  height: 50px;
}
</style>
