<template>
  <header id="start">
    <div class="img-wrapper">
      <img src="../images/bg-unsplash.jpg" alt="">
    </div>
    <div class="banner-wrapper">
      <div class="banner-text">
        <h2>DESENVOLVIMENTO FRONT-END</h2>
        <h3>Heron Nepomuceno</h3>
      </div>
      <div class="banner-button">
        <a href="#sobre">Começar!</a>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
      name: 'HeaderComp',
  }
</script>

<style>
  .header {
    width: 100%;
    height: 100vh;
    overflow: hidden;
    position: relative;
  }

  .img-wrapper {
    width: 100%;
    height: 100%;
    background: #000;
    overflow: hidden;
  }

  .img-wrapper > img {
    width: 100%;
    height: 100vh;
    object-fit: cover;
    opacity: .8;
    margin: 0;
    animation: zoom 2s;
  }

  @keyframes zoom {
    0%{
        transform: scale(1.3);
    }
    100%{
        transform: scale(1);
    }
  }

  .banner-wrapper {
    position: absolute;
    top: 40%;
    color: #f2e7fe;
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 99%;
    margin: auto;
    background-color: rgba(31, 31, 31, 0.5);
    padding: 1rem 0;
    margin-left: .15rem;
  }

  .banner-text {
    margin: 0 .76rem;
    margin-bottom: 2rem;
  }

  .banner-text h2 {
    font-family: var(--fontPrimary);
    font-size: 1.6rem;
  }

  .banner-text h3 {
    font-family:  var(--fontSecondary);
    font-size: 1rem;
  }

  .banner-button {
    display: flex;
    justify-content: flex-end;
    margin-right: .76rem;
  }

  .banner-button a {
    background: #B64FC8;
    padding: .72rem 2rem;
    border-radius: 10px;
    font-family: var(--fontSecondary);
    font-size: .86rem;
    color: #fff;
    transition: .5s all;
  }

  .banner-button a:hover{
    background: #6200ee;
  }

  .banner-button a:active{
    transform: scale(0.90);
  }


  @media (min-width:1025px) {
    .img-wrapper > img {
      width: 100%;
      height: 100vh;
      object-fit: cover;
      opacity: .8;
      margin: 0;
      animation: zoom 20s;
    }

    .banner-wrapper {
      position: absolute;
      color: #f2e7fe;
      display: flex;
      width: 100%;
      margin: 0;
      padding: 0;
      padding-top: 1.5rem;
      bottom: 0;
      top: 80%;
      background: rgba(31, 31, 31, 0);
      flex-direction: row;
      justify-content: space-between;
    }

    .banner-text {
      margin: 0 5rem;
      margin-bottom: 0;
    }

    .banner-text h2 {
      font-size: 2.5rem;
      text-shadow: #000 0.1em 0.1em 0.2em
    }

    .banner-text h3 {
      font-size: 1.5rem;
      text-shadow: #000 0.1em 0.1em 0.2em
    }

    .banner-button {
      display: flex;
      justify-content: flex-end;
      align-items: center;
      margin-right: 5rem;
    }

    .banner-button a {
      height: auto;
      padding: 1.2rem 4rem;
      font-size: 1.2rem;
      box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
    }
  }
</style>