<template>
<div>
    <div class="wrapper">
        <elevator-item />
        <floor-container />
    </div>
    
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
           
         
        }
    },
    methods:{
        // callElevator(index){
        //   console.log(index+1)
            
        //    }

        
    },
}
</script>

<style lang="scss">
body{
    box-sizing: border-box;
}

  #app {
    display: flex;
   
   /* font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    margin-top: 100px;
    
    position: relative;*/
} 
.wrapper{
   margin-top: 100px;
    margin-left: 100px;
}
</style>
