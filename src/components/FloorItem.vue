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
    width: 1000px;
    height: 137px;
 //   border: 2px solid #000000;
//margin-left: 125px;
    position: relative;
	border: 2px solid #000000;
	

  
}
</style>
