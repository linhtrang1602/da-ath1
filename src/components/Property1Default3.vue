<template>
  <div :class="$style.property1default" :style="property1Default2Style">
    <div :class="$style.groupSlideshow">
      <div :class="$style.groupSlideshowInner">
        <img :class="$style.frameChild" alt="" src="/rectangle-2@2x.png" />
      </div>
      <div :class="$style.groupSlideshowChild">
        <img :class="$style.frameChild" alt="" src="/rectangle-21@2x.png" />
      </div>
      <div :class="$style.frameDiv">
        <img :class="$style.frameChild" alt="" src="/rectangle-22@2x.png" />
      </div>
      <div :class="$style.groupSlideshowInner1">
        <img :class="$style.frameChild" alt="" src="/rectangle-23@2x.png" />
      </div>
      <div :class="$style.groupSlideshowInner2">
        <img :class="$style.frameChild" alt="" src="/rectangle-24@2x.png" />
      </div>
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";

  export default defineComponent({
    name: "Property1Default3",
    props: {
      property1DefaultPosition: { type: String },
      property1DefaultFlexShrink: { type: String },
    },
    computed: {
      property1Default2Style() {
        return {
          position: this.property1DefaultPosition,
          flexShrink: this.property1DefaultFlexShrink,
        };
      },
    },
  });
</script>
<style module>
  .frameChild {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 1440px;
    height: 512px;
    object-fit: cover;
  }
  .groupSlideshowInner {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 1440px;
    height: 512px;
  }
  .groupSlideshowChild {
    position: absolute;
    top: 0px;
    left: 5760px;
    width: 1440px;
    height: 512px;
  }
  .frameDiv {
    position: absolute;
    top: 0px;
    left: 1440px;
    width: 1440px;
    height: 512px;
  }
  .groupSlideshowInner1 {
    position: absolute;
    top: 0px;
    left: 2880px;
    width: 1440px;
    height: 512px;
    background-image: url("/public/frame-5@3x.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: top;
  }
  .groupSlideshowInner2 {
    position: absolute;
    top: 0px;
    left: 4320px;
    width: 1440px;
    height: 512px;
    background-image: url("/public/frame-6@3x.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: top;
  }
  .groupSlideshow {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 7200px;
    height: 512px;
  }
  .property1default {
    width: 1440px;
    height: 512px;
    overflow: hidden;
  }
</style>
