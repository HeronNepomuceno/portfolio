<template>
    <section class="section-wrapper">
      <div id="sobre" class="section-title">
          <h3>Sobre mim...</h3>
      </div>
      <div class="section-about-wrapper">
          <div class="section-about">
              <img src="../images/profile.jpg" alt="">
              <span>Olá, sou Heron, enquanto trabalho gosto de ouvir um lo-fi de qualidade e estar acompanhado de uma boa xícara de café. No tempo livre eu pratico ciclismo e sou entusiasta dos jogos.</span>
          </div>
      </div>
      <div class="separator-hr" id="about">
        <hr>  <!-- - - - - - - - - - - - - - - - SEPARADOR - - - - - - - - - - - - - - - - - - - -->
      </div>
    </section>
</template>

<script>
  export default {
    name: 'AboutComp'
  }
</script>

<style>
  #about {
    display: flex;
  }

  .section-about-wrapper {
    margin: 2rem 0;
  }

  .section-about {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 100%;
  }

  .section-about > img {
    width: 45%;
    border-radius: 50px;
    border: solid 1px #B64FC8;
    margin: 0 1rem;
  }

  .section-about > span {
    color: #fff;
    font-family: var(--fontSecondary);
  }

  @media (min-width:1025px) {
    .section-about > img {
      width: 20%;
    }

    #about {
      display: none;
    }

    .section-about > span {
      width: 50%;
      font-size: 1.2rem;
    }

    .section-about > img {
      margin: 0 .5rem;
    }
  }
</style>