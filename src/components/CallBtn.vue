<template>
<div>
    <div class="btn"></div>
</div>
</template>

<script>
export default {
    name: 'CallBtn',
    
    
}
</script>

<style lang="scss" scoped>
.btn{
    width: 40px;
    height: 40px;
    border: 2px solid rgb(0, 128, 0);
    border-radius: 5px;
    cursor: pointer;
    position: absolute;
    top: 35%;
    left: 10px;
    transition: .3s ease;

    &:hover{
        background-color: rgb(6, 207, 6);
    }

    &:active{
        background-color: rgb(0, 70, 0);
    }
}
</style>
