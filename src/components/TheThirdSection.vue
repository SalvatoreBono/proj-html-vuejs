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
  <section class="container pt-5 pb-5">
    <div class="text-center pb-4">
      <h6 class="fw-bold text-uppercase">the pericuros</h6>
      <h2 class="fw-bold text-uppercase">Meet the team</h2>
    </div>
    <div class="d-flex flex-wrap text-center gap-4">
      <div class="stucture-width-4">
        <img src="../assets/Team-01.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">Fabricio guerra</h4>
        <p class="text-secondary">Main Director</p>
      </div>
      <div class="stucture-width-4">
        <img src="../assets/Team-02.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">umberto pagoda</h4>
        <p class="text-secondary">Main Writer</p>
      </div>
      <div class="stucture-width-4">
        <img src="../assets/Team-03.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">gloria riccasso</h4>
        <p class="text-secondary">Main Producer</p>
      </div>
      <div class="stucture-width-4">
        <img src="../assets/Team-04.jpg" alt="" />
        <h4 class="fw-bold pt-4 pb-2 text-uppercase">Lio napoin</h4>
        <p class="text-secondary">Cameraman</p>
      </div>
    </div>
  </section>
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
        <p>
          Curabitur bindum ex ut sapien blandit viverra. Nunc lobortis mi dui,
          id Etiam tempor sit amet metus in bibendum. Nunc eros risus,
          pellentesque a augue pellentesque fringilla eget mi eu mollis.
          commodo.
        </p>
        <div class="d-flex justify-content-center">
          <div class="me-3">
            <img class="rounded-circle" src="../assets/01.jpg" alt="" />
          </div>
          <div class="d-flex flex-column text-start">
            <div class="text-uppercase fw-bold">John doe</div>
            <div class="small">Designer</div>
          </div>
        </div>
        <div class="pt-3">
          <i class="fa-solid fa-circle fa-2xs"></i>
          <i class="fa-solid fa-circle fa-2xs"></i>
          <i class="fa-solid fa-circle fa-2xs"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.stucture-width-4 {
  width: calc(100% / 4 - 2rem);
}
.stucture-width-4:hover img {
  transform: scale(1.05);
  transition: 0.5s;
}
.bg-about-us {
  background-image: url(../assets/Parallax-02.jpg);
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
}
.bg-about-us img {
  width: 60px;
}
</style>
