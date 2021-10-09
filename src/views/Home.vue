<template>
  <div class="home">

    <pubKeyboardContainer></pubKeyboardContainer>

    <div class="row" id="Keyboard">
      <div class="title">
        <h1>Les Nouveautés</h1>
      </div>
      <keyboardContainer></keyboardContainer>
    </div>
    
  </div>
</template>

<script>
// @ is an alias to /src
import keyboardContainer from "@/components/keyboardContainer.vue"
import pubKeyboardContainer from "@/components/pubKeyboardContainer.vue"

export default {
  name: 'Home',
  components: {
    keyboardContainer,
    pubKeyboardContainer
  }
}
</script>

<style scoped>  

.home {
  width: 100vw;
  height: 93vh;
  min-height: 93vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 2rem;
}

.row {
  display: flex;
  align-items: flex-starts;
  justify-content: center;
  flex-direction: row;
}

.title {
  width: 450px;
  height: 550px;
  background: url(../assets/img/keyboard.jpg);
  background-position: center;
  background-size: cover;
  border-radius: 20px;
  margin: 1rem;
  display: flex;
  align-items: flex-end;
}

.title h1 {
  font-size: 3rem;
  padding: 1.5rem;
}
</style>