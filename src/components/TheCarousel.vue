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
  <div class="card rounded-0 text-bg-dark position-relative">
    <img src="../assets/54863431.jpg" class="card-img" alt="..." />
    <div class="card-img-overlay d-flex align-items-center container">
      <div class="card-title text-uppercase">
        <h5 class="fw-bold">cinemato studio</h5>
        <h1 class="display-6 fw-bold">
          action and <br />
          inspire people
        </h1>
        <button
          type="button"
          class="rounded-0 fw-bold btn btn-light pe-4 ps-4 pt-2 pb-2 mt-5"
        >
          READ MORE
        </button>
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
</template>

<style lang="scss" scoped>
.btn-carousel {
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  display: flex;
  justify-content: space-between;
}
.btn-custom {
  background-color: rgba(0, 0, 0, 0.3);
  color: white;
  font-size: 20px;
  opacity: 0;
}

.card:hover .btn-custom {
  opacity: 1;
}
</style>
