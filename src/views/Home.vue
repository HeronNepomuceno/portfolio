<template>
  <div class="home">
    <HeaderComp/>
    <AboutComp/>
    <TechComp/>
    <PortComp/>
    <FooterComp/>
  </div>
</template>

<script>
  import HeaderComp from '../components/HeaderComp.vue';
  import AboutComp from '../components/AboutComp.vue';
  import TechComp from '../components/TechComp.vue';
  import PortComp from '../components/PortComp.vue';
  import FooterComp from '../components/FooterComp.vue';

  export default {
    components: {
      HeaderComp,
      AboutComp,
      TechComp,
      PortComp,
      FooterComp
    }
  }
</script>
