<template>
  <div :class="$style.main" data-scroll-to="mainContainer">
    <div :class="$style.picture">
      <div :class="$style.vectorParent">
        <img :class="$style.groupChild" alt="" src="/ellipse-6.svg" />
        <img :class="$style.artboard41" alt="" src="/artboard-4-1@2x.png" />
      </div>
    </div>
    <img :class="$style.maskGroupIcon" alt="" src="/mask-group@2x.png" />
    <div :class="$style.maskGroupParent">
      <img :class="$style.maskGroupIcon1" alt="" src="/mask-group1@2x.png" />
      <div :class="$style.recyclingAndWaste">
        Recycling and waste classification are simple ways to protect the
        environment. If you are concerned about waste classification, let us
        accompany you in environmental protection
      </div>
      <Property1Default4 />
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Property1Default4 from "./Property1Default4.vue";

  export default defineComponent({
    name: "Main",
    components: { Property1Default4 },
  });
</script>
<style module>
  .groupChild {
    position: absolute;
    top: 555.48px;
    left: 0px;
    width: 613.68px;
    height: 66.52px;
  }
  .artboard41 {
    position: absolute;
    top: 0px;
    left: calc(50% - 280.23px);
    width: 540.51px;
    height: 555.48px;
    object-fit: cover;
  }
  .vectorParent {
    position: absolute;
    top: 0px;
    left: 23px;
    width: 613.68px;
    height: 622px;
  }
  .picture {
    position: absolute;
    top: 0px;
    left: 606px;
    width: 655px;
    height: 772px;
  }
  .maskGroupIcon {
    position: absolute;
    top: 60px;
    left: 0px;
    width: 204px;
    height: 88px;
    object-fit: cover;
  }
  .maskGroupIcon1 {
    position: relative;
    width: 493px;
    height: 124px;
    object-fit: cover;
  }
  .recyclingAndWaste {
    position: relative;
    line-height: 35px;
    font-weight: 500;
    display: inline-block;
    width: 677px;
  }
  .maskGroupParent {
    position: absolute;
    top: 148px;
    left: 0px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-31xl);
  }
  .main {
    position: absolute;
    top: 154px;
    left: calc(50% - 657px);
    width: 1314px;
    height: 772px;
    text-align: left;
    font-size: var(--medium-18-spcline35-size);
    color: var(--color-black);
    font-family: var(--medium-18-spcline35);
  }
</style>
