<template>
<div>
    <h2>Current queue:{{queue}}</h2>
    <div class="floor-wrapper">
       
        <floor-item v-for="(floor, index) in floors" :key="floor.id" @callElevator="callElevator(index)">
            <span class="floor-number">{{index + 1}}</span>
        </floor-item>
    </div>
</div>
</template>

<script>
import FloorItem from "@/components/FloorItem";
//import { toRaw } from '@vue/reactivity';
export default {
    name: 'FloorContainer',
    components: {
        FloorItem
    },
    data() {
        return {
            queue: [],
            floors: [1, 2, 3, 4, 5],

        }

    },
    // props:{
    //     floors:Array,
    // },
    methods: {
        callElevator(index) {
            
         this.queue.push(index + 1);
        //  console.log(toRaw(this.queue))
           return (this.queue);
          

        }

    },
   
    
}
</script>

<style lang="scss" scoped>
.floor {
    &-wrapper {
        height: 700px;
        width: auto;
        display: flex;
        flex-direction: column-reverse;
        //justify-content: space-between;
        //  margin-top: 20px;
        position: absolute;
       top: 85px;
      left: 240px;
      //  border: 2px solid #000000;
      
    
    }

    &-number {
        display: block;
        font-size: 20px;
        font-weight: 600;
        margin: 10px;
    }

    

    
}
</style>
