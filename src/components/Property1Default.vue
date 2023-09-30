<template>
  <div :class="$style.property1default" :style="property1DefaultStyle">
    <div :class="$style.letsClassify">Let’s classify</div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";

  export default defineComponent({
    name: "Property1Default",
    props: {
      property1DefaultPosition: { type: String },
      property1DefaultTop: { type: [Object, Array, String, Number, Boolean] },
      property1DefaultLeft: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      property1DefaultStyle() {
        return {
          position: this.property1DefaultPosition,
          top: this.property1DefaultTop,
          left: this.property1DefaultLeft,
        };
      },
    },
  });
</script>
<style module>
  .letsClassify {
    position: relative;
    letter-spacing: 0.05em;
    font-weight: 600;
  }
  .property1default {
    border-radius: var(--br-mini);
    background-color: var(--color-seagreen);
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-3xs) var(--padding-xl);
    text-align: left;
    font-size: var(--medium-18-spcline35-size);
    color: var(--color-white);
    font-family: var(--medium-18-spcline35);
  }
</style>
