<template>
    <div class="flex justify-center my-12 ">
        <span class="rounded-full border-2 p-2 text-[#4f7df3] text-2xl hover:bg-[#4f7df3] hover:text-white hover:transition-colors duration-700 hover:ease-in-out">
            <slot></slot>
        </span>
    </div>
</template>
<script>
export default {
    props: [],
    components: { SocialComponent }
}
</script>
<style >
    
</style>