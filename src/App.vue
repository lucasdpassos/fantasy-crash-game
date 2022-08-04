<template>
  <div>
    <div class="bg-primary w-screen h-screen">
      <div class="flex align-top justify-center w-[400px] h-[300px] m-auto">
        <img src="./assets/char.gif" />
      </div>
      <div>
        <div class="bg-secondary w-[800px] h-[400px]  border-4 border-indigo-200 border-l-[white] m-auto">
          <div v-if="menu" class="flex flex-col items-center">
        <button @click="menu = false;play = true" class="bg-secondary w-56 hover:opacity-20 text-[white] mt-6 border-[white] border-4">Começar</button>
        <button @click="menu = false" class="bg-secondary w-56 hover:opacity-20 text-[white] mt-6 border-[white] border-4">Regras</button>
        </div>
        <StartGame v-if="play" />
        </div>
      </div>
    </div>
  </div>
 
</template>

<script>
import StartGame from './components/StartGame.vue'

export default {
  data() {
    return {
      play: false,
      menu: true
    }
  },
  components: {
    StartGame
  }
 
}
</script>