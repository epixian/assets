<template>
    <div>
        <h1 class="font-normal font-3xl text-grey-darkest leading-none">
            Loaders & Animations
        </h1>

        <div ref="lottie" class="w-64" style="height: 457px"></div>
    </div>

</template>

<script>
import lottie from 'lottie-web';

export default {
    // mounted() {
    //     lottie.loadAnimation({
    //         container: this.$refs.lottie,
    //         renderer: 'svg',
    //         loop: true,
    //         autoplay: true,
    //         path: '/animations/spinner.json'
    //     });
    // }

};
</script>
