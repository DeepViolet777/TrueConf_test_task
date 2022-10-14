<template>
<div>
    <elevator-item />
    <floor-container/>
</div>
</template>

<script>
import ElevatorItem from "@/components/ElevatorItem";
import FloorContainer from "@/components/FloorContainer";

export default {
    name: 'App',
    components: {
        ElevatorItem,
        FloorContainer
    },
    data() {
        return {
            
           
            queuqe: [],
            elevator: {
                currentFloor: 1,
                isMoving: false,
                isRefreshing: false
            },
        }
    },
    methods:{
        callElevator(index){
          console.log(index+1)
            
           }

        
    },
}
</script>

<style lang="scss">


/* #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
} */
</style>
