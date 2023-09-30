<template>
  <div :class="$style.memberssProfile" :style="memberssProfileStyle">
    <div :class="$style.ellipseParent" :style="frameDivStyle">
      <img :class="$style.frameChild" alt="" :src="imageDimensions" />
      <div :class="$style.trnhThNgcAnhParent">
        <div :class="$style.trnhThNgc">{{personAvatarUrl}}</div>
        <div :class="$style.frameParent">
          <div :class="$style.fluentmail16RegularParent">
            <img
              :class="$style.fluentmail16RegularIcon"
              alt=""
              :src="imageDimensionsUrl"
            />
            <div :class="$style.ngocem0601gmailcom">{{emailAvatarUrl}}</div>
          </div>
          <div :class="$style.phphoneLightParent">
            <img
              :class="$style.fluentmail16RegularIcon"
              alt=""
              :src="imageDimensionsText"
            />
            <div :class="$style.ngocem0601gmailcom">{{phoneNumber}}</div>
          </div>
          <div :class="$style.iconoirdiscordParent">
            <img
              :class="$style.fluentmail16RegularIcon"
              alt=""
              :src="imageDimensionsTextUrl"
            />
            <div :class="$style.ngocem0601gmailcom">{{userAvatarUrl}}</div>
          </div>
        </div>
      </div>
    </div>
    <Property1Variant3
      group1="/group-12.svg"
      property1Variant3Position="absolute"
      property1Variant3Top="483px"
      property1Variant3Left="calc(50% - 16px)"
    />
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Property1Variant3 from "./Property1Variant3.vue";

  export default defineComponent({
    name: "MemberssProfile",
    components: { Property1Variant3 },
    props: {
      imageDimensions: { type: String },
      personAvatarUrl: { type: String },
      imageDimensionsUrl: { type: String },
      emailAvatarUrl: { type: String },
      imageDimensionsText: { type: String },
      phoneNumber: { type: String },
      imageDimensionsTextUrl: { type: String },
      userAvatarUrl: { type: String },
      imageDimensionsText2: { type: String },
      propLeft: { type: [Object, Array, String, Number, Boolean] },
      propLeft1: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      memberssProfileStyle() {
        return {
          left: this.propLeft,
        };
      },
      frameDivStyle() {
        return {
          left: this.propLeft1,
        };
      },
    },
  });
</script>
<style module>
  .frameChild {
    position: relative;
    border-radius: 50%;
    width: 378px;
    height: 378px;
    object-fit: cover;
  }
  .trnhThNgc {
    position: relative;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    font-weight: 600;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #484848;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .fluentmail16RegularIcon {
    position: relative;
    width: 28px;
    height: 28px;
    overflow: hidden;
    flex-shrink: 0;
  }
  .ngocem0601gmailcom {
    position: relative;
    line-height: 35px;
    font-weight: 500;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #484848;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .fluentmail16RegularParent {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-11xl);
  }
  .phphoneLightParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-11xl);
  }
  .iconoirdiscordParent {
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: flex-start;
    gap: var(--gap-11xl);
  }
  .frameParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    font-size: var(--medium-18-spcline35-size);
  }
  .trnhThNgcAnhParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-51xl);
  }
  .ellipseParent {
    position: absolute;
    top: 71px;
    left: calc(50% - 444px);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    gap: var(--gap-101xl);
  }
  .memberssProfile {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 1440px;
    height: 520px;
    text-align: left;
    font-size: var(--semib-32-size);
    font-family: var(--medium-18-spcline35);
  }
</style>
