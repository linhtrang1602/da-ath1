<template>
  <div :class="$style.product" data-scroll-to="productContainer">
    <div :class="$style.ourProduct">OUR PRODUCT</div>
    <div :class="$style.frameParent">
      <frame
        productImageUrl="/frame-12.svg"
        featureDescription="Easy To Use"
        productDescription="A simple, user-friendly interface ensures you have the best experience with the product."
      /><frame
        productImageUrl="/frame-11.svg"
        featureDescription="Environmentally friendly"
        productDescription="With a simple interface and superior features, DA ATH's products always protect the environment."
        propWidth="414px"
      /><frame
        productImageUrl="/frame-9.svg"
        featureDescription="Convenient"
        productDescription="Providing accurate and fast information about waste types to help you sort easily."
        propWidth="unset"
      />
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Frame from "./Frame.vue";

  export default defineComponent({
    name: "Product",
    components: { Frame },
  });
</script>
<style module>
  .ourProduct {
    position: relative;
    letter-spacing: 0.05em;
    line-height: 35px;
    font-weight: 600;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #126128;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .frameParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-123xl);
    font-size: var(--b-30-size);
  }
  .product {
    position: absolute;
    top: 2045px;
    left: calc(50% - 601px);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-56xl);
    text-align: center;
    font-size: var(--semib-32-size);
    color: var(--color-darkslategray);
    font-family: var(--medium-18-spcline35);
  }
</style>
