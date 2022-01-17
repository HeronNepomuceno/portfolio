<template>
  <section>
    <div class="section-title">
      <h3>Portfólio...</h3>
    </div>
    <div class="section-subtitle">
      <span>Website para empresa</span>
    </div>

    <div class="section-img">
      <img src="../images/maejr1.png">
    </div>

    <div id="slider-maejr">
      <figure>
        <img src="../images/maejr1.png">
        <img src="../images/maejr2.png">
        <img src="../images/maejr3.png">
      </figure>
    </div>
    <div class="banner-button banner-button--slide">
      <a v-bind:href="link_maejr" target="_blank">{{ portButton }}</a>
    </div>
    <div class="section-info section-info--slide">
      <span>O cliente desejava um website para expandir sua identidade visual, dessa forma foi feito um website utilizando das cores, fontes e logo da empresa, com um design claro, objetivo e também responsivo.</span>
    </div>
    <div class="section-acess">
      <a v-bind:href="link_maejr" target="_blank">Clique aqui para visitar o projeto.</a>
    </div>

    <div class="separator-hr">
      <hr>  <!-- - - - - - - - - - - - - - - - SEPARADOR - - - - - - - - - - - - - - - - - - - -->
    </div>

    <div class="section-subtitle">
      <span>Jogo de Perguntas e Respostas</span>
    </div>

    <div class="section-img">
      <img src="../images/atecair1.png">
    </div>

    <div id="slider-atecair">
      <figure>
        <img src="../images/atecair1.png">
        <img src="../images/atecair2.png">
      </figure>
    </div>
    <div class="banner-button banner-button--slide">
      <a v-bind:href="link_atecair" target="_blank">{{ portButton }}</a>
    </div>
    <div class="section-info section-info--slide">
      <span>Esse projeto foi solicitado amistosamente em um grupo de amigos que desejavam formas de entreter o público na festa que haveria no dia. Dessa forma foi feito um jogo de perguntas e respostas envolvendo bebidas.</span>
    </div>
    <div class="section-acess">
      <a v-bind:href="link_atecair" target="_blank">Clique aqui para visitar o projeto.</a>
    </div>

    <div class="separator-hr">
      <hr>  <!-- - - - - - - - - - - - - - - - SEPARADOR - - - - - - - - - - - - - - - - - - - -->
    </div>

    <div class="section-download">
      <span>Clique no ícone para baixar o Portfólio do Programador.</span>
      <div class="download-icon">
        <a href="#" target="_blank">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-file-earmark-pdf-fill" viewBox="0 0 16 16">
            <path d="M5.523 12.424c.14-.082.293-.162.459-.238a7.878 7.878 0 0 1-.45.606c-.28.337-.498.516-.635.572a.266.266 0 0 1-.035.012.282.282 0 0 1-.026-.044c-.056-.11-.054-.216.04-.36.106-.165.319-.354.647-.548zm2.455-1.647c-.119.025-.237.05-.356.078a21.148 21.148 0 0 0 .5-1.05 12.045 12.045 0 0 0 .51.858c-.217.032-.436.07-.654.114zm2.525.939a3.881 3.881 0 0 1-.435-.41c.228.005.434.022.612.054.317.057.466.147.518.209a.095.095 0 0 1 .026.064.436.436 0 0 1-.06.2.307.307 0 0 1-.094.124.107.107 0 0 1-.069.015c-.09-.003-.258-.066-.498-.256zM8.278 6.97c-.04.244-.108.524-.2.829a4.86 4.86 0 0 1-.089-.346c-.076-.353-.087-.63-.046-.822.038-.177.11-.248.196-.283a.517.517 0 0 1 .145-.04c.013.03.028.092.032.198.005.122-.007.277-.038.465z"/>
            <path fill-rule="evenodd" d="M4 0h5.293A1 1 0 0 1 10 .293L13.707 4a1 1 0 0 1 .293.707V14a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V2a2 2 0 0 1 2-2zm5.5 1.5v2a1 1 0 0 0 1 1h2l-3-3zM4.165 13.668c.09.18.23.343.438.419.207.075.412.04.58-.03.318-.13.635-.436.926-.786.333-.401.683-.927 1.021-1.51a11.651 11.651 0 0 1 1.997-.406c.3.383.61.713.91.95.28.22.603.403.934.417a.856.856 0 0 0 .51-.138c.155-.101.27-.247.354-.416.09-.181.145-.37.138-.563a.844.844 0 0 0-.2-.518c-.226-.27-.596-.4-.96-.465a5.76 5.76 0 0 0-1.335-.05 10.954 10.954 0 0 1-.98-1.686c.25-.66.437-1.284.52-1.794.036-.218.055-.426.048-.614a1.238 1.238 0 0 0-.127-.538.7.7 0 0 0-.477-.365c-.202-.043-.41 0-.601.077-.377.15-.576.47-.651.823-.073.34-.04.736.046 1.136.088.406.238.848.43 1.295a19.697 19.697 0 0 1-1.062 2.227 7.662 7.662 0 0 0-1.482.645c-.37.22-.699.48-.897.787-.21.326-.275.714-.08 1.103z"/>
          </svg>
        </a>
      </div>
    </div>

  </section>
</template>

<script>
  export default {
      name: 'PortComp',
      data() {
        return {
          portButton: 'Visite o projeto',
          link_maejr: 'https://maejr.netlify.app/',
          link_atecair: 'https://atecair.netlify.app/'
        }
      }
  }
</script>

<style>

  .section-subtitle {
    background: #1F1F1F;
    padding: .7rem;
    margin: 2rem 0;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .section-subtitle > span {
    color: #fff;
    font-family: var(--fontSecondary);
    font-size: 1.2rem;
  }

  .section-info--slide {
    margin: 0;
    padding: .7rem 1rem;
  }

  .banner-button--slide {
    justify-content: center;
    align-items: center;
    margin: 2rem 0;
  }

  .section-acess {
    display: none;
  }

  .section-img {
    display: none;
  }

/* - - - - - - - - - - SLIDE DO PROJETO MAEJR - - - - - - - - - - */

  #slider-maejr {
    overflow: hidden;
  }

  #slider-maejr figure{
    position: relative;
    width: 500%;
    margin: 0;
    left: 0;
    animation: 10s slider-maejr infinite;
  }

  #slider-maejr figure img {
    width: 20%;
    float: left;
  }

@keyframes slider-maejr {
  0% {
    left: 0;
  }
  20% {
    left: 0;
  }
  25% {
    left: -100%;
  }
  45% {
    left: -100%;
  }
  50% {
    left: -200%;
  }
  70% {
    left: -200%;
  }
}

/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - */

/* - - - - - - - - - - SLIDE DO PROJETO ATECAIR - - - - - - - - - - */

#slider-atecair {
    overflow: hidden;
  }

  #slider-atecair figure{
    position: relative;
    width: 500%;
    margin: 0;
    left: 0;
    animation: 10s slider-atecair infinite;
  }

  #slider-atecair figure img {
    width: 20%;
    float: left;
  }

@keyframes slider-atecair {
  0% {
    left: 0;
  }
  20% {
    left: 0;
  }
  25% {
    left: -100%;
  }
  45% {
    left: -100%;
  }
}

/* - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - */

  .section-download {
    background: #1F1F1F;
    padding: 1rem 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }

  .section-download > span {
    color: #fff;
    font-family: var(--fontSecondary);
    font-size: 1.2rem;
    margin-bottom: 1rem;
  }

  .download-icon {
    background: #383838;
    border-radius: 15px;
    margin-left: 1rem;
  }

  .download-icon > a > svg{
    margin: 1rem .5rem 1rem .5rem;
    width: 46px;
    height: 46px;
    color: #B64FC8;
    transition: .5s all;
  }

  .download-icon > a > svg:hover {
    color: #c80a0a;
    transform: scale(1.1);
  }

  @media (min-width:1025px) {
    .section-subtitle {
      margin: 0;
      margin-bottom: 2rem;
      padding: 1rem 1rem;
    }

    .section-subtitle > span{
      font-size: 1.4rem;
    }

    .section-img {
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .banner-button--slide {
      display: none;
    }

    .section-info--slide {
      margin: 2rem 0;
    }

    .section-acess {
      display: block;
      background: #1F1F1F;
      padding: 1rem;
      margin: 3rem 0 1rem 0;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .section-acess > a {
      font-family: var(--fontSecondary);
      color: #B64FC8;
      font-size: 1.2rem;
      transition: .5s all;
    }

    .section-acess > a:hover{
      color: #6200ee;
    }

    #slider-maejr {
      display: none;
    }

    #slider-atecair {
      display: none;
    }
      
  }

</style>