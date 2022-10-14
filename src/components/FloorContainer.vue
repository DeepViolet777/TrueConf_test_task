<template>
<div>
    <div class="floor-wrapper">
        <floor-item v-for="(floor, index) in floors" :key="floor.id" @callElevator="callElevator(index)">
            <span class="floor-number">{{index + 1}}</span>
        </floor-item>
    </div>
</div>
</template>

<script>
import FloorItem from "@/components/FloorItem";
export default {
    name: 'FloorContainer',
    components: {
        FloorItem
    },
    data() {
        return {
            floors: [1, 2, 3, 4, 5],
        }

    },
    methods: {
        callElevator(index) {
            console.log(index + 1)

        }

    },
}
</script>

<style lang="scss" scoped>

.floor {
    &-wrapper {
        height: 90vh;
        width: auto;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        margin-top: 20px;
    }

    &-number {
        display: block;
        font-size: 20px;
        font-weight: 600;
        margin: 10px;
    }
}

</style>
