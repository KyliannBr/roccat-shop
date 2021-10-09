<template>

  <div class="container">
        <video autoplay muted loop>
            <source src="../assets/video/videoplayback.mp4">
        </video>
  </div>

</template>


<script>
export default {
    name: 'pubKeyboardContainer',
    props: {
        video: String
    }   
};
</script>


<style scoped>

.container {
    position: relative;
    width: calc(450px + 2rem + 1200px);
    height: 550px;
    margin: 1rem;
    border-radius: 20px;
    overflow: hidden;
  }

  video {
    width: 100%;
    position: relative;
    transform: translateY(-20%);
  }

</style>