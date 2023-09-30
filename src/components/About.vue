<template>
  <div :class="$style.about" data-scroll-to="aboutContainer">
    <Property1Default3
      property1DefaultPosition="relative"
      property1DefaultFlexShrink="0"
    />
    <div :class="$style.bothWeAndYouCareAboutTheParent">
      <div :class="$style.bothWeAnd">
        Both we and you care about the environment
      </div>
      <div :class="$style.weUnderstandHow">
        We understand how important nature is to humanity. Now more than ever,
        it's a time for us to realize the importance of environmental
        protection. Please don't think of it as too big of an issue. We can
        protect the environment through simple daily actions: waste sorting. “I
        don't know which types of waste can be recycled and which cannot!” Don't
        worry, let DA ATH help you with waste classifycation.
      </div>
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";
  import Property1Default3 from "./Property1Default3.vue";

  export default defineComponent({
    name: "About",
    components: { Property1Default3 },
  });
</script>
<style module>
  .bothWeAnd {
    position: relative;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    font-weight: 600;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #126128;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .weUnderstandHow {
    position: relative;
    font-size: var(--medium-18-spcline35-size);
    letter-spacing: 0.05em;
    line-height: 35px;
    text-align: center;
    display: inline-block;
    width: 1247px;
  }
  .bothWeAndYouCareAboutTheParent {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-31xl);
  }
  .about {
    position: absolute;
    top: 1051px;
    left: calc(50% - 720px);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-81xl);
    text-align: left;
    font-size: var(--semib-32-size);
    color: var(--color-black);
    font-family: var(--medium-18-spcline35);
  }
</style>
