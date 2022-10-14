<template>
<div>
    <div class="elevator-shaft">
        <div class="elevator-cabin"></div>
    </div>
</div>
</template>

<script>
export default {
    name: 'ElevatorItem',
}
</script>

<style lang="scss" scoped>
.elevator{
    &-shaft{
        width: 100px;
        height: 90vh;
        border: 2px solid #000000;
        position: absolute;
        left: 30px;
        top: 20px;
    }

    &-cabin{
        width: 100px;
        height: 140px;
        background-color: rgb(25, 126, 241);
        margin: 0 auto;
    }
}
</style>
