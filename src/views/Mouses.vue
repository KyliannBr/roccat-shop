<template>
  <div class="mouses">


        <small>ROCCAT Gaming Burst Pro</small>
        <h1>Created by gamers for gamers</h1>
        <p class="titleDesc">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iure nemo consequuntur blanditiis soluta beatae, provident voluptatem nostrum ullam molestiae quasi architecto excepturi eius incidunt accusamus minus dolorum natus corrupti dicta.</p>
        <p class="prix">a partir de 45,99€</p>
        <button class="buyIt">Acheter</button>

        <img src="../assets/img/mouseMainPic.jpg" alt="" class="mainPic">

        <div class="grilleProducts">  
            <CardProducts productImg="../assets/img/keyboard.jpg"></CardProducts>
        </div>

        <h1></h1>
  </div>
</template>

<script>
// @ is an alias to /src
import CardProducts from "@/components/CardProducts.vue"


export default {
  name: 'Mouses',
  components: {
    CardProducts
  }
}
</script>

<style scoped>  

@font-face {
    font-family: Glitch;
    src: url(../assets/font/Doctor_Glitch.otf);
  }

  .mouses {
    min-height: 93vh;
    background-color: #000000;
    display: flex;
    flex-direction: column;
    position: relative;
    justify-content: flex-start;
    align-items: center;
    color: rgb(255, 255, 255);
  }

  small {
    padding: 4rem 0 0 0;
    font-size: 1.3rem;
    font-weight: 500;
  }

  h1 {
    font-size: 3.5rem;
  }

  .titleDesc {
     padding: 1rem; 
     width: 550px;
     text-align: center;
     font-size: 1.3rem;
  }

  .prix {
    font-size: 1.3rem;
    padding: 2rem;
    color: rgb(51, 51, 51);
  }

  .buyIt {
    background-color: var(--bluetiful);
    border: none;
    padding: .7rem 1.7rem;
    border-radius: 999px;
    color: #fff;
    font-weight: 500;
    font-size: 1.1rem;
  }

  .mainPic {
    width: 100%;
    height: auto;
    bottom: 0;
  }

  .grilleProducts {

  }
  
</style>