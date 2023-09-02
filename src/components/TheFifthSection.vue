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
  <div class="container pt-5 pb-5">
    <div class="row">
      <div class="col-6">
        <h6 class="fw-bold">COLLABORATE</h6>
        <h1 class="fw-bold pt-2 pb-4">
          WANT TO WORK WITH US? <br />
          LEAVE US A MESSAGE!
        </h1>
        <p class="collaborate">
          Duis sit amet congue ipsum. Nulla maximus My venenatis posuere.To The
          Mauris ut tempus Suspendisse porta tincidunt lectus non of me
          pellentesque. At A Sed blandit at diam sit amet Orci varius natoque
          penatibus et dis dis to parturient montes, My Car nascetur ridiculus
          Sed feugiat lacus in erat egestas, quis eleifend lacus imperdiet.
        </p>
      </div>
      <div class="col-6">
        <div class="d-flex gap-4">
          <input
            class="ps-3 w-100 pt-2 pb-2 border-0 form"
            type="text"
            name=""
            placeholder="Your Name"
            id=""
          />
          <input
            class="ps-3 w-100 pt-2 pb-2 border-0 form"
            type="text"
            name=""
            placeholder="Your email"
            id=""
          />
        </div>
        <div class="d-flex pt-5 gap-4">
          <input
            class="ps-3 w-100 pt-2 pb-2 border-0 form"
            type="text"
            name=""
            placeholder="Mobile number"
            id=""
          />
          <input
            class="ps-3 w-100 pt-2 pb-2 border-0 form"
            type="text"
            name=""
            placeholder="Your Pincode"
            id=""
          />
        </div>
        <div class="d-flex flex-column">
          <textarea
            class="form border-0 mt-5 ps-3 pt-2 pb-2 pe-5"
            name=""
            id=""
            placeholder="Enter Your Message"
            rows="6"
          ></textarea>
          <button type="button" class="mt-5 rounded-0 btn btn-dark fw-bold">
            SUBMIT NOW
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.form {
  background-color: rgb(242, 242, 242);
  font-size: 1.1rem;
}
.collaborate {
  color: rgb(102, 102, 102);
  text-align: justify;
}
input:focus {
  outline: none;
}
textarea:focus {
  outline: none;
}
</style>
