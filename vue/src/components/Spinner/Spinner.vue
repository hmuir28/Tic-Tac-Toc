<template>
  <div v-if="loading">
    <svg width="200px"  height="200px"  xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="xMidYMid" class="lds-reload" style="background: none;">
      <g transform="rotate(252 50 50)">
        <path d="M50 15A35 35 0 1 0 74.787 25.213" fill="none" stroke="#68d3e6" stroke-width="12"></path>
        <path d="M49 3L49 27L61 15L49 3" fill="#68d3e6"></path>
        <animateTransform attributeName="transform" type="rotate" calcMode="linear" values="0 50 50;360 50 50" keyTimes="0;1" dur="1s" begin="0s" repeatCount="indefinite"></animateTransform>
      </g>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'Spinner',

  props: {
    loading: {
      default: false,
      type: Boolean,
    }
  }
}
</script>
