<template>
  <div :class="$style.frameParent">
    <img :class="$style.frameChild" alt="" :src="productImageUrl" />
    <div :class="$style.easyToUseParent">
      <b :class="$style.easyToUse" :style="easyToUseStyle"
        >{{featureDescription}}</b
      >
      <div :class="$style.aSimpleUserFriendly">{{productDescription}}</div>
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";

  export default defineComponent({
    name: "Frame",
    props: {
      productImageUrl: { type: String },
      featureDescription: { type: String },
      productDescription: { type: String },
      propWidth: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      easyToUseStyle() {
        return {
          width: this.propWidth,
        };
      },
    },
  });
</script>
<style module>
  .frameChild {
    position: relative;
    border-radius: var(--br-31xl) 0px var(--br-31xl) 0px;
    width: 100px;
    height: 100px;
  }
  .easyToUse {
    position: relative;
    letter-spacing: 0.05em;
    line-height: 35px;
  }
  .aSimpleUserFriendly {
    position: relative;
    font-size: var(--medium-18-spcline35-size);
    letter-spacing: 0.05em;
    line-height: 35px;
    color: var(--color-black);
    display: inline-block;
    width: 252px;
  }
  .easyToUseParent {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-11xl);
  }
  .frameParent {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-21xl);
    text-align: center;
    font-size: var(--b-30-size);
    color: var(--color-darkslategray);
    font-family: var(--medium-18-spcline35);
  }
</style>
