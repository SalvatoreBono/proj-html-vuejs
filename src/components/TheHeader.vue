<script>
import TheCarousel from "./TheCarousel.vue";
export default {
  components: {
    TheCarousel,
  },
  data() {
    return {};
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <nav class="navbar pe-5 bg-white ps-5">
    <div class="container-fluid d-flex">
      <div>
        <a class="navbar-brand" href="#">
          <img
            src="../assets/logo.svg"
            alt="Bootstrap"
            width="200"
            height="75"
          />
        </a>
      </div>
      <div class="d-flex justify-content-center flex-grow-1">
        <ul class="navbar-nav flex-row text-uppercase">
          <li class="nav-item pe-5">
            <a class="nav-link" href="#">home</a>
          </li>
          <li class="nav-item pe-5">
            <a class="nav-link" href="#">blog</a>
          </li>
          <li class="nav-item dropdown pe-5">
            <a class="nav-link d-flex align-items-end" href="#"
              >Pages <i class="ps-1 fa-solid fa-angle-down"></i>
            </a>
            <ul class="hover-nav list-unstyled pe-5 list-group">
              <li>
                <a class="dropdown-item list-group-item" href="#">services</a>
              </li>
              <li>
                <a class="dropdown-item list-group-item" href="#"
                  >our work flow</a
                >
              </li>
              <li>
                <a class="dropdown-item list-group-item" href="#"
                  >video thumbnail type</a
                >
              </li>
            </ul>
          </li>
          <li class="nav-item pe-5">
            <a class="nav-link" href="#">about</a>
          </li>
          <li class="nav-item pe-5">
            <a class="nav-link" href="#">contacts</a>
          </li>
          <li class="nav-item pe-5">
            <a class="nav-link" href="#">gallery</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link d-flex align-items-end" href="#"
              >shop <i class="ps-1 fa-solid fa-angle-down"></i>
            </a>
            <ul class="hover-nav list-unstyled pe-5 list-group">
              <li>
                <a class="dropdown-item list-group-item" href="#">Shop pages</a>
              </li>
              <li>
                <a class="dropdown-item list-group-item" href="#"
                  >product type</a
                >
              </li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="d-flex align-items-center">
        <i class="fa-solid fa-magnifying-glass fa-xl pe-3"></i>
        <div class="line border-end"></div>
        <i class="fa-brands fa-facebook-f fa-lg"></i>
        <i class="fa-brands fa-twitter fa-lg"></i>
        <i class="fa-brands fa-youtube fa-lg"></i>
        <i class="fa-brands fa-instagram fa-lg"></i>
      </div>
    </div>
  </nav>
  <TheCarousel></TheCarousel>
</template>

<style lang="scss" scoped>
ul li {
  font-weight: 700;
}
.navbar {
  position: fixed;
  width: 100%;
  z-index: 1000;
}

.hover-nav {
  position: absolute;
  display: none;
  top: 65px;
}

.hover-nav li a {
  color: white;
  padding-right: 7rem;
  font-weight: 700;
  background-color: black;
}
i {
  padding-left: 1.3rem;
}
.line {
  height: 30px;
}
.dropdown:hover .hover-nav {
  display: block;
}
</style>
