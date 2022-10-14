<template>
<div>
    <!-- <div class="floor-container"> -->
    <div class="floor">
        <slot></slot>
        <call-btn @click="callElevator" />
    </div>

</div>
</template>

<script>
import CallBtn from "@/components/CallBtn";
export default {
    name: 'FloorItem',
    components: {
        CallBtn
    },
    methods:{
        callElevator(){
        this.$emit('callElevator');
        }
    }
}
</script>

<style lang="scss" scoped>
.floor {
    width: 90vw;
    height: 140px;
    border: 2px solid #000000;
    margin-left: 125px;
    position: relative;

    &-container {
        height: 170px;
        width: auto;
        margin-top: 20px;

    }
}
</style>
