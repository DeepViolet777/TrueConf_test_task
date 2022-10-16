<template>
<div>
    <div class="elevator-shaft">
        <div class="elevator-cabin floor-1"></div>
    </div>
</div>
</template>

<script>
export default {
    name: 'ElevatorItem',
    data() {
        // elevator: {
        //     currentFloor: 1;
        //     isMoving: false;
        //     isRefreshing: false;
        // }
    }
}
</script>

<style lang="scss" scoped>
.elevator {
    &-shaft {
        width: 100px;
        height: 700px;
        border: 2px solid #000000;
        position: relative;
        left: 30px;
        top: -28px;
    }

    &-cabin {
        width: 100px;
        height: 140px;
        background-color: rgb(25, 126, 241);
        //   position: absolute;
        transition: translateY .2s ease;

    }

}

.level-1 {
    transform: translateY(400%);
}

.level-2 {
    transform: translateY(300%);
}

.level-3 {
    transform: translateY(200%);
}

.level-4 {
    transform: translateY(100%);
}

.level-5 {
    transform: translateY(0);
}
</style>
