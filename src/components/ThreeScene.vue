<template>
    <div class="threeScene">
        <div class="container" ref="container"></div>
    </div>
</template>

<script>
import MainThreeScene from "@/classes/MainThreeScene";

export default {
    name: "HelloWorld",
    props: {
        msg: String,
    },
    mounted() {
        MainThreeScene.init(this.$refs.container);
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.threeScene {
    position: absolute;
    top: 0;
    left: 0;
    // pointer-events: none;
}</style>
