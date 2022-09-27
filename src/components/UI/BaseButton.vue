<template>
  <button :type="type" :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['type', 'mode'],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #700c07;
  border: 1px solid #700c07;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #8c100a;
  border-color: #8c100a;
}

.flat {
  background-color: transparent;
  color: #700c07;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #f5ebeb;
}
</style>
