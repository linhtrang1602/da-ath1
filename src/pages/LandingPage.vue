<template>
  <div :class="$style.landingPage">
    <div :class="$style.landingPageChild" />
    <main />
    <About /><Product /><Property1Default2
      phphoneLight="/phphonelight2.svg"
      iconoirdiscord="/iconoirdiscord5.svg"
      phphoneLight1="/phphonelight3.svg"
      iconoirdiscord1="/iconoirdiscord6.svg"
      phphoneLight2="/phphonelight4.svg"
      iconoirdiscord2="/iconoirdiscord7.svg"
      phphoneLight3="/phphonelight4.svg"
      iconoirdiscord3="/iconoirdiscord8.svg"
      phphoneLight4="/phphonelight4.svg"
      iconoirdiscord4="/iconoirdiscord9.svg"
      phphoneLight5="/phphonelight4.svg"
      iconoirdiscord5="/iconoirdiscord9.svg"
      property1DefaultFlexShrink="unset"
      property1DefaultPosition="absolute"
      property1DefaultTop="2627px"
      property1DefaultLeft="calc(50% - 720px)"
    /><Contact /><MainMenu />
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Main from "../components/Main.vue";
  import About from "../components/About.vue";
  import Product from "../components/Product.vue";
  import Property1Default2 from "../components/Property1Default2.vue";
  import Contact from "../components/Contact.vue";
  import MainMenu from "../components/MainMenu.vue";

  export default defineComponent({
    name: "LandingPage",
    components: { Main, About, Product, Property1Default2, Contact, MainMenu },
  });
</script>
<style module>
  .landingPageChild {
    position: absolute;
    top: calc(50% - 511.5px);
    left: calc(50% - 720px);
    background-color: var(--color-white);
    width: 1440px;
    height: 1024px;
  }
  .landingPage {
    position: relative;
    background-color: var(--color-white);
    width: 100%;
    height: 3749px;
    overflow: hidden;
  }
</style>
