<template>
  <form class="py-10 w-10/12  mx-auto" @submit.prevent>
    <div class="mb-3">
      <input
        type="email"
        name="email"
        id="email"
        ref="email"
        placeholder="Your email address"
        class="block rounded-3xl text-sm px-5 py-3 border border-solid border-[#969696] w-full"
        :style="isError && emailBorderStyle"
      />
      <p v-show="isError" class="text-[#ff5263] italic text-sm">
        Please provide a valid email address
      </p>
    </div>

    <input
      type="submit"
      value="Notify Me"
      class="block bg-[#4f7df3] text-white rounded-3xl text-sm py-3 shadow-lg shadow-[#c2d3ff] border-2 border-[#c2d3ff]  w-full"
      @click="showError"
    />
  </form>
</template>
<script>
export default {
  data() {
    return {
      isError: false,
      emailBorderStyle: { borderColor: "#ff5263" },
    };
  },
  methods: {
    showError() {
      let emailVal = this.$refs.email;
      var filter =
        /^([a-zA-Z0-9_\.\-])+\@(([a-zA-Z0-9\-])+\.)+([a-zA-Z0-9]{2,4})+$/;

      !filter.test(emailVal.value)
        ? (this.isError = true)
        : (this.isError = false);
    },
  },
};
</script>
