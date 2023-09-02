<script>
export default {
  components: {},
  data() {
    return {
      Footer: [
        {
          title: `information`,
          credits: [
            `Product Support`,
            `Checkout`,
            `Report Abuse`,
            `Redeem Voucher`,
            `Order Status`,
          ],
        },
        {
          title: `useful links`,
          credits: [
            `Policies & Rules`,
            `Privacy Policy`,
            `License Policy`,
            `My Account`,
            `Locality`,
          ],
        },
      ],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<template>
  <section
    style="padding-top: 70px; background-color: rgb(17, 17, 17)"
    class="text-white"
  >
    <footer class="container pt-5 pb-5">
      <div class="d-flex flex-wrap gap-5">
        <div class="stucture-width-4">
          <h5 class="text-uppercase fw-bold pb-3">Contact info</h5>
          <ul class="list-unstyled">
            <li class="pb-2">
              <a
                class="text-footer text-decoration-none d-flex align-items-baseline"
                href=""
              >
                <i class="fa-solid fa-location-dot me-3"></i>
                <div>2/45 Tower Street, New York USA</div></a
              >
            </li>

            <li class="pb-2">
              <a class="text-footer text-decoration-none" href=""
                ><i class="fa-solid fa-phone me-3"></i> Call us on 0800 840
                1010</a
              >
            </li>
            <li class="pb-2">
              <a class="text-footer text-decoration-none" href="">
                <i class="fa-solid fa-envelope me-3"></i>Demo@Example.com</a
              >
            </li>
          </ul>
        </div>
        <div v-for="singleFooter in Footer" class="stucture-width-4">
          <h5 class="text-uppercase fw-bold pb-3">{{ singleFooter.title }}</h5>
          <ul class="list-unstyled">
            <li v-for="singleCredits in singleFooter.credits" class="pb-2">
              <a class="text-footer text-decoration-none" href="">{{
                singleCredits
              }}</a>
            </li>
          </ul>
        </div>

        <div class="stucture-width-4">
          <h5 class="text-uppercase fw-bold pb-4">newsletter</h5>
          <p style="color: rgb(102, 102, 102)">
            Subscribe to receive inspiration, ideas & News in your inbox.
          </p>
          <input
            style="background-color: rgb(28, 28, 28); font-size: 20px"
            class="ps-3 w-100 pt-3 pb-3 border-0"
            type="text"
            name=""
            placeholder="Enter Your Email"
            id=""
          />
          <button
            type="button"
            class="rounded-0 fw-bold btn btn-light pe-5 ps-5 pt-3 pb-3 mt-4"
          >
            SUBSCRIBE
          </button>
        </div>
      </div>
      <hr style="margin-top: 150px" />
      <div
        style="color: rgb(102, 102, 102); font-size: 18px"
        class="text-center pt-3"
      >
        © 2023 All Rights Reserved. Developed By TemplateMela
      </div>
    </footer>
  </section>
</template>

<style lang="scss" scoped>
.stucture-width-4 {
  width: calc(100% / 4 - 3rem);
}
.text-footer {
  color: rgb(102, 102, 102);
  font-size: 1.2rem;
}

.text-footer:hover {
  color: white;
  transition: 0.5s;
}
input:focus {
  outline: none;
  caret-color: white;
}
input::placeholder {
  color: rgb(102, 102, 102);
}
</style>
