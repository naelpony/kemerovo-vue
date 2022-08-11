<template >
  <svg
    class="iconsvg"
    xmlns="http://www.w3.org/2000/svg"
    :width="width"
    :height="height"
    :aria-labelledby="iconName"
    :viewBox="viewBox"
    fill="none"
    role="presentation"
  >
    <path
      d="M5 55H55"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M30 5C34 6.6 38.5 6.6 42.5 5V12.5C38.5 14.1 34 14.1 30 12.5V5Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M30 12.5V20"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M42.5 20H17.5C12.5 20 10 22.5 10 27.5V55H50V27.5C50 22.5 47.5 20 42.5 20Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M10 30L50 30"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M19.9746 30V55"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linejoin="round"
    />
    <path
      d="M29.9746 30V55"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linejoin="round"
    />
    <path
      d="M39.9746 30V55"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-miterlimit="10"
      stroke-linejoin="round"
    />
  </svg>
</template>
<script>
export default {
  props: {
    iconName: {
      type: String,
      default: "box",
    },
    width: {
      type: [Number, String],
      default: 18,
    },
    height: {
      type: [Number, String],
      default: 18,
    },
    viewBox: {
      type: [Number, String],
      default: "0 0 18 18",
    },
    iconColor: {
      type: String,
      default: "currentColor",
    },
  },
};
</script>
<style lang="sass">
</style>