<template>
    <div class="flex justify-center my-12 ">
        <!-- <SocialComponent/> -->
        <span class="flex rounded-full border-2 p-2 text-blue-600 text-2xl hover:bg-blue-600 hover:text-white">
            <slot></slot>
        </span>
    </div>
</template>
<script>
import SocialComponent from './sub/SocialComponent.vue';

export default {
    props: [],
    components: { SocialComponent }
}
</script>
<style >
    
</style>