<script>
export default {
  components: {},
  data() {
    return {
      news: [
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
        {
          img: `blog03.jpg`,
          date: ` April 10 , 2022 By Admin`,
          title: `last video website you need for`,
          overview: ` Is as name to here them deny wise this. As rapid woody my he me which. Men but they fail shew just`,
        },
        {
          img: `blog04.jpg`,
          date: ` March 01 , 2022 By Admin`,
          title: `Band uprising to cult status`,
          overview: ` Porta tellus aliquam ligula sollicitudin tindidunt habitant egestas erat lectus congue nisl`,
        },
        {
          img: `blog05.jpg`,
          date: ` February 14, 2022 By Admin`,
          title: `Bringing the stage to life`,
          overview: `Actor The Concept Movie High Concept Theory see the post As Clover Letter  Emails Got`,
        },
        {
          img: `blog06.jpg`,
          date: ` December 07 , 2021 By Admin`,
          title: `cadenze rios picked for the next picture`,
          overview: ` inhabit hearing perhaps on ye do no. It maids decay as there he. Smallest on suitable disposed do`,
        },
      ],
      logos: [
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
  methods: {
    btnRight() {
      /* this.$refs.containerCards è il container delle carte */
      const wrapper = this.$refs.containerCards;

      /* this.$refs.singleCard[0] prende la singola carta */
      const card = this.$refs.singleCard[0];

      /* card.OffsetWidth prende la Width della carta */
      /*  wrapper.scrollLeft scrolla a destra utilizzando la grandezza della carta */
      wrapper.scrollLeft += card.offsetWidth + 16;
    },
    btnLeft() {
      const wrapper = this.$refs.containerCards;

      const card = this.$refs.singleCard[0];

      /*  wrapper.scrollLeft scrolla a sinistra -(la grandezza della carta) */
      wrapper.scrollLeft -= card.offsetWidth;
    },
  },
  mounted() {},
};
</script>

<template>
  <!-- START FOURTH SECTION -->

  <section class="pb-5">
    <div class="container news pt-5 position-relative">
      <div class="text-center">
        <h6 class="fw-bold text-uppercase">Latest news</h6>
        <h3 class="fw-bold pb-4 pt-3 text-uppercase">articles updated daily</h3>
      </div>
      <div
        class="d-flex gap-3 justify-content-between custom-carousel"
        ref="containerCards"
      >
        <!-- START FOR -->

        <div
          v-for="singleNews in news"
          class="structure flex-shrink-0"
          ref="singleCard"
        >
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
        <!-- END FOR -->
      </div>
      <div class="btn-carousel">
        <button
          @click="btnLeft()"
          type="button"
          class="btn btn-custom rounded-0 ms-3"
        >
          <i class="fa-solid fa-chevron-left"></i>
        </button>
        <button
          @click="btnRight()"
          type="button"
          class="btn btn-custom rounded-0 me-3"
        >
          <i class="fa-solid fa-chevron-right"></i>
        </button>
      </div>
    </div>
  </section>
  <!-- END FOURTH SECTION -->

  <!-- START BANNER LOGO -->

  <section class="pt-5 pb-5">
    <div class="bg-photo d-flex align-items-center">
      <div class="container text-white">
        <div class="d-flex flex-wrap">
          <!-- START FOR -->
          <div v-for="SingleLogos in logos" class="stucture-width-5">
            <img :src="`src/assets/${SingleLogos.img}`" alt="" />
          </div>
          <!-- END FOR -->
        </div>
      </div>
    </div>
  </section>
  <!--END BANNER LOGO -->
</template>

<style lang="scss" scoped>
.structure {
  width: calc(100% / 3 - 1rem);
}
.structure img {
  width: 100%;
}
.custom-carousel {
  overflow-x: hidden;
  scrollbar-width: none;
  scroll-behavior: smooth;
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
  background-attachment: fixed;
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
