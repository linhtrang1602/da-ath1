<template>
  <div :class="$style.property1variant3" :style="property1Variant3Style">
    <img :class="$style.property1variant3Child" alt="" :src="group1" />
  </div>
</template>
<script>
  import { defineComponent, ref } from "vue";

  export default defineComponent({
    name: "Property1Variant3",
    props: {
      group1: { type: String },
      property1Variant3Position: { type: String },
      property1Variant3Top: { type: [Object, Array, String, Number, Boolean] },
      property1Variant3Left: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      property1Variant3Style() {
        return {
          position: this.property1Variant3Position,
          top: this.property1Variant3Top,
          left: this.property1Variant3Left,
        };
      },
    },
  });
</script>
<style module>
  .property1variant3Child {
    position: relative;
    width: 32px;
    height: 8px;
  }
  .property1variant3 {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
  }
</style>
