<template >
  <svg
    class="iconsvg"
    xmlns="http://www.w3.org/2000/svg"
    :width="width"
    :height="height"
    :aria-labelledby="iconName"
    :viewBox="viewBox"
		fill=none
    role="presentation"
  >
    <path
      d="M45.0002 17.9C44.8502 17.875 44.6752 17.875 44.5252 17.9C41.0752 17.775 38.3252 14.95 38.3252 11.45C38.3252 7.875 41.2002 5 44.7752 5C48.3502 5 51.2252 7.9 51.2252 11.45C51.2002 14.95 48.4502 17.775 45.0002 17.9Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M42.4256 36.0999C45.8506 36.6749 49.6256 36.0749 52.2756 34.2999C55.8006 31.9499 55.8006 28.0999 52.2756 25.7499C49.6006 23.9749 45.7756 23.3749 42.3506 23.9749"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M14.9242 17.9C15.0742 17.875 15.2492 17.875 15.3992 17.9C18.8492 17.775 21.5992 14.95 21.5992 11.45C21.5992 7.875 18.7242 5 15.1492 5C11.5742 5 8.69922 7.9 8.69922 11.45C8.72422 14.95 11.4742 17.775 14.9242 17.9Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M17.4996 36.0999C14.0746 36.6749 10.2996 36.0749 7.64961 34.2999C4.12461 31.9499 4.12461 28.0999 7.64961 25.7499C10.3246 23.9749 14.1496 23.3749 17.5746 23.9749"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M30.0002 36.5748C29.8502 36.5498 29.6752 36.5498 29.5252 36.5748C26.0752 36.4498 23.3252 33.6248 23.3252 30.1248C23.3252 26.5498 26.2002 23.6748 29.7752 23.6748C33.3502 23.6748 36.2252 26.5748 36.2252 30.1248C36.2002 33.6248 33.4502 36.4748 30.0002 36.5748Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
    <path
      d="M22.7248 44.4499C19.1998 46.7999 19.1998 50.6499 22.7248 52.9999C26.7248 55.6749 33.2748 55.6749 37.2748 52.9999C40.7998 50.6499 40.7998 46.7999 37.2748 44.4499C33.2998 41.7999 26.7248 41.7999 22.7248 44.4499Z"
      stroke="#F4F4F4"
      stroke-width="3"
      stroke-linecap="round"
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
      default:'0 0 18 18',
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