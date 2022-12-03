<template>
  <form
    class="py-10 w-10/12 mx-auto md:flex md:justify-between md:max-w-xl"
    @submit.prevent
  >
    <span class="mb-3 block md:inline-block">
      <input
        type="email"
        name="email"
        id="email"
        ref="email"
        placeholder="Your email address"
        class="block rounded-3xl text-sm px-5 py-3 border border-solid border-[#969696] w-full md:w-96"
        :style="isError && emailBorderStyle"
      />
      <p
        v-show="isError"
        class="text-[#ff5263] italic text-sm md:text-left md:pl-5"
      >
       {{errorMessage}}
      </p>
    </span>
    <span>
      <input
        type="submit"
        value="Notify Me"
        class="block bg-[#4f7df3] text-white rounded-3xl text-sm py-3 shadow-lg shadow-[#c2d3ff] border-2 border-[#c2d3ff] w-full cursor-pointer hover:bg-[#c2d3ff] duration-300 hover:transition-colors hover:ease-in-out md:w-44"
        @click="showError"
      />
    </span>
  </form>
</template>
<script>
export default {
  data() {
    return {
      isError: false,
      emailBorderStyle: { borderColor: "#ff5263" },
      errorMessage: "",
    };
  },
  methods: {
    showError() {
      let emailVal = this.$refs.email;
      var filter =
        /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/;
      
        if (emailVal.value === "") {
          this.errorMessage = "Whoops! It looks like you forgot to add your email";
          this.isError = true;
        } else if (!filter.test(emailVal.value)) {
          this.errorMessage = "Please provide a valid email address";
          this.isError = true;
        } else {
          this.isError = false;
        }
    },
  },
};
</script>
