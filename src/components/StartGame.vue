<template>
    <div class="container flex justify-center items-center bg-white h-[400px]">
         <video class=" relative opacity-60 max-h-[700px] max-w-[700px]" autoplay loop muted>
            <source src="../assets/game-bg.mp4" type="video/mp4" />
                       
        </video>
        <img class="z-50 mr-44 absolute max-w-[200px] animate-pulse" src="../assets/sword.png" />
        
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    },
     props: {
    play: Boolean
  } 
}
</script>