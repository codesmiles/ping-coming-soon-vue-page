<template>
    <div style="color:red;font-size:larger" class="flex justify-center my-12">
        <!-- <SocialComponent/> -->
        <span class="flex rounded-full border-2">
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