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
  <section class="pb-5">
    <div class="container news pt-5 position-relative">
      <div class="text-center">
        <h6 class="fw-bold text-uppercase">Latest news</h6>
        <h3 class="fw-bold pb-4 pt-3 text-uppercase">articles updated daily</h3>
      </div>
      <div class="row justify-content-between">
        <div class="structure">
          <img src="../assets/blog07.jpg" alt="" />
          <div class="pt-3 pb-3 text-secondary small">
            November 06 , 2021 By Admin
          </div>
          <h6 class="fw-bold pb-2 text-uppercase">
            recap your latest company event
          </h6>
          <p class="small">
            Suspendisse dictum dictum tempor.Ut non faucibus arcu, id elementum
            est. Suspendisse sed
          </p>
        </div>
        <div class="structure">
          <img src="../assets/blog01.jpg" alt="" />
          <div class="pt-3 pb-3 text-secondary small">
            May 27 , 2022 By Admin
          </div>
          <h6 class="fw-bold pb-2 text-uppercase">
            how to edit a film score to serve
          </h6>
          <p class="small">
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laudantium
            placeat sed harum
          </p>
        </div>
        <div class="structure">
          <img src="../assets/blog02.jpg" alt="" />
          <div class="pt-3 pb-3 text-secondary small">
            May 07 , 2022 By Admin
          </div>
          <h6 class="fw-bold pb-2 text-uppercase">
            are you ready to make it awesome
          </h6>
          <p class="small">
            Design is our playground. While we create an awesome experience, we
            like having fun. No animals
          </p>
        </div>
      </div>
      <div class="btn-carousel">
        <button type="button" class="btn btn-custom rounded-0 ms-3">
          <i class="fa-solid fa-chevron-left"></i>
        </button>
        <button type="button" class="btn btn-custom rounded-0 me-3">
          <i class="fa-solid fa-chevron-right"></i>
        </button>
      </div>
    </div>
  </section>
  <section class="pt-5 pb-5">
    <div class="bg-photo d-flex align-items-center">
      <div class="container text-white">
        <div class="d-flex flex-wrap">
          <div class="stucture-width-5">
            <img src="../assets/03.png" alt="" />
          </div>
          <div class="stucture-width-5">
            <img src="../assets/04.png" alt="" />
          </div>
          <div class="stucture-width-5">
            <img src="../assets/05.png" alt="" />
          </div>
          <div class="stucture-width-5">
            <img src="../assets/01.png" alt="" />
          </div>
          <div class="stucture-width-5">
            <img src="../assets/02.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.structure {
  width: calc(100% / 3);
}
.structure img {
  width: 100%;
}
img:hover {
  transform: scale(1.05);
  transition: 0.5s;
}
.btn-carousel {
  position: absolute;
  top: 50%;
  left: -50px;
  right: -50px;
  display: flex;
  justify-content: space-between;
  opacity: 0;
}
.news:hover .btn-carousel {
  opacity: 1;
}
.bg-photo {
  background-image: url(../assets/Parallax-03.jpg);
  width: 100%;
  height: 250px;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.stucture-width-5 {
  width: calc(100% / 5);
}
</style>
