<template>
  <button :type="type" :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['type', 'mode'],
}
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  background-color: #3a0061;
  border: 1px solid #3a0061;
  color: white;
  cursor: pointer;
}
button:hover,
button:active {
  background-color: #270041;
  border-color: #270041;
}
.flat {
  background-color: transparent;
  color: #909090;
  border: 1px solid #909090;
  width: 100%;
}
.flat:hover,
.flat:active {
  background-color: #edd2ff;
  color: black;
}
</style>
