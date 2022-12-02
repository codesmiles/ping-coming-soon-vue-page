<template>
  <form class="py-10">
    <div class="mb-3">

      <input
        type="email"
        name="email"
        id="email"
        ref="email"
        placeholder="Your email address"
        class="block w-10/12 mx-auto rounded-3xl text-sm px-5 py-3 border border-solid border-[#969696] border-"
      />
      <p v-show="isError" class="text-[#ff5263] italic text-sm">Please provide a valid email address</p>
    </div>

    <input
      type="submit"
      value="Notify Me"
      class="block w-10/12 bg-[#4f7df3] text-white rounded-3xl text-sm py-3 shadow-lg shadow-[#c2d3ff] border border-2 border-[#c2d3ff] mx-auto"
      @click="showError"
    />
  </form>
</template>
<script>
export default {
  data() {
    return {
      isError:false
    }
  },
  methods: {
    showError(){
      // console.log(this.$refs.email.value)
    }
  },
};
</script>

