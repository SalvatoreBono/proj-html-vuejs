<script>
export default {
  components: {},
  data() {
    return {
      News: [
        {
          img: `blog07.jpg`,
          date: ` November 06 , 2021 By Admin`,
          title: `recap your latest company event`,
          overview: ` Suspendisse dictum dictum tempor.Ut non faucibus arcu, id elementum
            est. Suspendisse sed`,
        },
        {
          img: `blog01.jpg`,
          date: `  May 27 , 2022 By Admin`,
          title: ` how to edit a film score to serve`,
          overview: ` Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laudantium
            placeat sed harum`,
        },
        {
          img: `blog02.jpg`,
          date: ` May 07 , 2022 By Admin`,
          title: `are you ready to make it awesome`,
          overview: ` Design is our playground. While we create an awesome experience, we
            like having fun. No animals`,
        },
      ],
      Logos: [
        {
          img: `03.png`,
        },
        {
          img: `04.png`,
        },
        {
          img: `05.png`,
        },
        {
          img: `01.png`,
        },
        {
          img: `02.png`,
        },
      ],
    };
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
        <div v-for="singleNews in News" class="structure">
          <div class="animation">
            <img
              class="latest-news"
              :src="`src/assets/${singleNews.img}`"
              alt=""
            />
          </div>
          <div class="pt-3 pb-3 text-secondary small">
            {{ singleNews.date }}
          </div>
          <h6 class="fw-bold pb-2 text-uppercase">
            {{ singleNews.title }}
          </h6>
          <p class="small">
            {{ singleNews.overview }}
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
          <div v-for="SingleLogos in Logos" class="stucture-width-5">
            <img :src="`src/assets/${SingleLogos.img}`" alt="" />
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

.latest-news {
  transition: 0.5s;
}
.animation {
  overflow: hidden;
}
.latest-news:hover {
  transform: scale(1.05);
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
