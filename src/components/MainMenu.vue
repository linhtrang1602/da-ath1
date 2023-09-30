<template>
  <div :class="$style.mainMenu">
    <div :class="$style.mainMenuChild" />
    <div :class="$style.mainMenu1">
      <b :class="$style.daAth">DA ATH</b>
      <div :class="$style.mainParent">
        <div :class="$style.main" :onClick="onMainTextClick">Main</div>
        <div :class="$style.main" :onClick="onAboutTextClick">About</div>
        <div :class="$style.main" :onClick="onProductTextClick">Product</div>
        <div :class="$style.main" :onClick="onMembersTextClick">Members</div>
        <div :class="$style.main" :onClick="onContactTextClick">Contact</div>
      </div>
      <Property1Default
        property1DefaultPosition="absolute"
        property1DefaultTop="0px"
        property1DefaultLeft="1096px"
      />
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Property1Default from "./Property1Default.vue";

  export default defineComponent({
    name: "MainMenu",
    components: { Property1Default },
    methods: {
      onMainTextClick() {
        const anchor = document.querySelector(
          "[data-scroll-to='mainContainer']"
        );
        if (anchor) {
          anchor.scrollIntoView({ block: "start", behavior: "smooth" });
        }
      },
      onAboutTextClick() {
        const anchor = document.querySelector(
          "[data-scroll-to='aboutContainer']"
        );
        if (anchor) {
          anchor.scrollIntoView({ block: "start", behavior: "smooth" });
        }
      },
      onProductTextClick() {
        const anchor = document.querySelector(
          "[data-scroll-to='productContainer']"
        );
        if (anchor) {
          anchor.scrollIntoView({ block: "start", behavior: "smooth" });
        }
      },
      onMembersTextClick() {
        const anchor = document.querySelector(
          "[data-scroll-to='frameMemberContainer']"
        );
        if (anchor) {
          anchor.scrollIntoView({ block: "start", behavior: "smooth" });
        }
      },
      onContactTextClick() {
        const anchor = document.querySelector(
          "[data-scroll-to='contactContainer']"
        );
        if (anchor) {
          anchor.scrollIntoView({ block: "start", behavior: "smooth" });
        }
      },
    },
  });
</script>
<style module>
  .mainMenuChild {
    position: relative;
    background-color: var(--color-white);
    width: 1440px;
    height: 77px;
    z-index: 0;
  }
  .daAth {
    position: absolute;
    top: 6.5px;
    left: 0px;
  }
  .main {
    position: relative;
    font-weight: 500;
    cursor: pointer;
  }
  .mainParent {
    position: absolute;
    top: 10px;
    left: calc(50% - 245px);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-21xl);
    font-size: var(--medium-18-spcline35-size);
    color: var(--color-black);
  }
  .mainMenu1 {
    position: absolute;
    margin: 0 !important;
    top: 17px;
    left: 58px;
    width: 1264px;
    height: 42px;
    z-index: 1;
  }
  .mainMenu {
    position: absolute;
    top: 0px;
    left: calc(50% - 720px);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-3xs);
    text-align: left;
    font-size: var(--font-size-5xl);
    color: var(--color-darkgreen);
    font-family: var(--medium-18-spcline35);
  }
</style>
