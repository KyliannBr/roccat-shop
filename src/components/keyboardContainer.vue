<template>

  <div class="container">
    <div class="clip clip1">
      <div class="content">

        <h2>Roccat Magma</h2>
        <p>
          Le clavier à membrane RGB ROCCAT® Magma est parfait pour les amateurs de RGB qui recherchent une dimension compétitive.
        </p>
        <a href="#">En savoir plus</a>
      </div>
    </div>
    <div class="clip clip2">
      <div class="content">
        <h2>Roccat Vulcan 122 AIMO</h2>
        <p>
          Cet outil gaming de précision dévoile ses performances dès le premier coup d'œil et la première frappe.
        </p>
        <a href="#">En savoir plus</a>
      </div>
    </div>
    <div class="clip clip3">
      <div class="content">
        <h2>Roccat Pyro</h2>
        <p>
          Le clavier mécanique RGB ROCCAT® Pyro est destiné aux joueurs ambitieux prêts à rejoindre le clan mécanique.
        </p>
        <a href="#">En savoir plus</a>
      </div>
    </div>
  </div>

</template>


<script>
export default {

};
</script>


<style scoped>

.container {
    position: relative;
    width: 1200px;
    height: 550px;
    background: radial-gradient(circle, rgba(255,255,255,1) 0%, rgba(57,58,102,1) 0%, rgba(0,0,0,1) 100%);
    margin: 1rem;
    border-radius: 20px;
  }

  .container .clip {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transition: all 0.5s;
  }

  .container .clip1 {
    background: url(../assets/img/img1.png);
    background-size: cover;
    background-position: center;
    clip-path: polygon(0 0, 40% 0, 20% 100%, 0% 100%);
  }

  .container .clip2 {
    background: url(../assets/img/img2.png);
    background-size: cover;
    background-position: center;
    clip-path: polygon(40% 0, 60% 0, 80% 100%, 20% 100%);
  }
  .container .clip3 {
    background: url(../assets/img/img3.png);
    background-size: cover;
    background-position: center;
    clip-path: polygon(60% 0, 100% 0, 100% 100%, 80% 100%);
  }

  .container:hover .clip {
    clip-path: polygon(100% 0, 100% 0, 100% 100%, 100% 100%);
  }

  .container .clip:hover {
    clip-path: polygon(0 0, 100% 0, 100% 100%, 0 100%);
  }

  .content {
    position: absolute;
    bottom: 0;
    bottom: -10%;
    width: 70%;
    height: 20vh;
    padding: 20px;
    background: #ffffffd8;
    opacity: 0;
    transition: 0.5s;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    color: var(--rich-black);
  }

  .clip:hover .content {
    bottom: 0;
    opacity: 1;
  }

  .content .close-btn img{
      width: 20px;
      position: absolute;
      right: 20px;
      top: 20px;
  }

  .content h2 {
      text-transform: uppercase;
  }

  .content p {
      font-size: calc(17 * var(--res));
      color: #000000;
  }

  .content a {
      border: 1px solid #fff;
      background-color: #1276b9;
      color: #fff;
      padding: 1vh 2vw;
      border-radius: 20px;
      width: auto;
      text-decoration: none;
      font-size: calc(15 * var(--res));
  }

</style>