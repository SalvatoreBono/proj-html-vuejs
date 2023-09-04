<script>
export default {
  components: {},
  data() {
    return {
      peliculaStudios: [
        {
          img: `image (14).svg`,
          title: `ARRAY OF EQUIPMENT`,
        },
        {
          img: `image (16).svg`,
          title: `NEW TECHNOLOGIES`,
        },
        {
          img: `image (18).svg`,
          title: `Versitile actors `,
        },
        {
          img: `image (15).svg`,
          title: `Top Directors `,
        },
        {
          img: `image (17).svg`,
          title: `Minute Editing `,
        },
        {
          img: `image (19).svg`,
          title: `Versitile actors `,
        },
      ],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <!-- START FIRST SECTION -->
  <section class="pt-5 pb-5">
    <div class="container text-center pt-5">
      <h6 class="fw-bold">PELICULA STUDIO</h6>
      <h3 class="fw-bold pb-5 pt-3">THIS IS WHAT WE DO</h3>
      <div class="row justify-content-between">
        <!-- START FOR -->
        <div v-for="singlePeliculaStudio in peliculaStudios" class="structure">
          <img :src="`../src/assets/${singlePeliculaStudio.img}`" alt="" />
          <h4 class="fw-bold pt-4 pb-2 text-uppercase">
            {{ singlePeliculaStudio.title }}
          </h4>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus eos,
            provident recusandae velit
          </p>
        </div>
        <!-- END FOR -->
      </div>
    </div>
  </section>

  <!-- START BANNER ABOUT US -->
  <section class="bg-about-us mb-5 d-flex align-items-center">
    <div
      class="container justify-content-center align-items-end d-flex flex-column text-white"
    >
      <div class="col-6">
        <h6 class="fw-bold">ABOUT US</h6>
        <h1 class="fw-bold pb-3">HIGH QUALITY CINEMATICS</h1>
        <p>
          Orci varius penatibus et magnis dis parturient in the montes, nascetur
          ridiculus mus. Nulla a nisi ut mi efficitur hendrerit. nunc urna.
          quisque a partr hendrerit purus erat, nec dapibus sem sed. phasellus
          sed elis molestie, portttor ligula of the egestas, mattis augue.
          quisque et rhoncus justo. suspendisse luctus pharetra eleme
          tcondimentum.
        </p>
        <button
          type="button"
          class="rounded-0 fw-bold btn btn-light pe-4 ps-4 pt-2 pb-2 mt-4"
        >
          READ MORE
        </button>
      </div>
    </div>
  </section>
  <!-- END BANNER ABOUT US -->
</template>

<style lang="scss" scoped>
.structure {
  width: calc(100% / 3 - 2rem);
  padding-bottom: 3rem;
}
.structure img {
  transition: 0.5s;
}
.structure:hover img {
  transform: translateY(-8px);
}
.structure img {
  width: 80px;
  height: 80px;
}
.bg-about-us {
  background-image: url(../assets/About-Us.jpg);
  width: 100%;
  height: 600px;
  background-size: contain;
  background-repeat: no-repeat;
}
</style>
