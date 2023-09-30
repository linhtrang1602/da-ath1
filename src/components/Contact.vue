<template>
  <div :class="$style.contact" data-scroll-to="contactContainer">
    <div :class="$style.frameMainMenu">
      <div :class="$style.frameMainMenuChild" />
      <div :class="$style.frameParent">
        <div :class="$style.contactUsNowParent">
          <b :class="$style.contactUsNow">Contact us now</b>
          <div :class="$style.biinstagramParent">
            <img
              :class="$style.biinstagramIcon"
              alt=""
              src="/biinstagram.svg"
            />
            <img :class="$style.biinstagramIcon" alt="" src="/lafacebook.svg" />
            <img
              :class="$style.biinstagramIcon"
              alt=""
              src="/iconoirdiscord10.svg"
            />
          </div>
        </div>
        <div :class="$style.getStartedNoewTryOurProduParent">
          <div :class="$style.getStartedNoew">
            Get started noew try our product
          </div>
          <div :class="$style.enterYourEmailHereParent">
            <div :class="$style.enterYourEmail">Enter your email here</div>
            <div :class="$style.groupChild" />
            <div :class="$style.groupItem" />
            <img
              :class="$style.arrowRight11Icon"
              alt=""
              src="/arrowright1-1.svg"
            />
          </div>
        </div>
      </div>
      <b :class="$style.biccas">Biccas</b>
    </div>
    <div :class="$style.thankYouForYourInterestInParent">
      <div :class="$style.thankYouFor">
        Thank you for your interest in our product.
      </div>
      <div :class="$style.theProductIsContainer">
        <p :class="$style.theProductIs">The product is designed to serve the</p>
        <p :class="$style.theProductIs">SheCodes Hackathon 2023 competition.</p>
      </div>
    </div>
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";

  export default defineComponent({
    name: "Contact",
  });
</script>
<style module>
  .frameMainMenuChild {
    position: absolute;
    top: 0px;
    left: calc(50% - 720px);
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #36a248;
    width: 1440px;
    height: 290px;
  }
  .contactUsNow {
    position: relative;
    letter-spacing: 0.05em;
    line-height: 35px;
  }
  .biinstagramIcon {
    position: relative;
    width: 36px;
    height: 36px;
    overflow: hidden;
    flex-shrink: 0;
  }
  .biinstagramParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-31xl);
  }
  .contactUsNowParent {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-21xl);
  }
  .getStartedNoew {
    position: absolute;
    top: 0px;
    left: 0px;
    line-height: 30px;
    font-weight: 500;
    display: inline-block;
    width: 286px;
  }
  .enterYourEmail {
    position: absolute;
    top: 15px;
    left: 20px;
    line-height: 30px;
    font-weight: 500;
    display: inline-block;
    width: 184px;
  }
  .groupChild {
    position: absolute;
    top: 0px;
    left: 0px;
    border-radius: var(--br-51xl);
    border: 2px solid var(--color-white);
    box-sizing: border-box;
    width: 410px;
    height: 60px;
  }
  .groupItem {
    position: absolute;
    top: 7px;
    left: 357px;
    border-radius: 50%;
    background-color: var(--color-mediumaquamarine);
    width: 46px;
    height: 46px;
  }
  .arrowRight11Icon {
    position: absolute;
    top: 18px;
    left: 368px;
    width: 24px;
    height: 24px;
    overflow: hidden;
  }
  .enterYourEmailHereParent {
    position: absolute;
    top: 60px;
    left: 0px;
    width: 410px;
    height: 60px;
  }
  .getStartedNoewTryOurProduParent {
    position: relative;
    width: 410px;
    height: 120px;
    font-size: var(--medium-18-spcline35-size);
    font-family: var(--font-inter);
  }
  .frameParent {
    position: absolute;
    top: 120px;
    left: 85px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-594xl);
  }
  .biccas {
    position: absolute;
    top: 63px;
    left: 85px;
    font-size: var(--b-50-size);
    line-height: 30px;
  }
  .frameMainMenu {
    position: absolute;
    top: 217px;
    left: 0px;
    width: 1440px;
    height: 290px;
  }
  .thankYouFor {
    position: relative;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    font-weight: 600;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #126128;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  .theProductIs {
    margin: 0;
  }
  .theProductIsContainer {
    position: relative;
    font-size: var(--font-size-5xl);
    letter-spacing: 0.05em;
    line-height: 35px;
    font-weight: 500;
    background: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), #484848;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-align: center;
    display: inline-block;
    width: 892px;
  }
  .thankYouForYourInterestInParent {
    position: absolute;
    top: 0px;
    left: 252px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: var(--gap-31xl);
    font-size: var(--semib-32-size);
  }
  .contact {
    position: absolute;
    bottom: 0px;
    left: calc(50% - 720px);
    width: 1440px;
    height: 507px;
    text-align: left;
    font-size: var(--b-30-size);
    color: var(--color-white);
    font-family: var(--medium-18-spcline35);
  }
</style>
