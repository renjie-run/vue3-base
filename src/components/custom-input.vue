<template>
  <input
    type="text"
    v-model="searchValue"
    @input="$emit('update:searchValue', $event.target.value)"
  />
</template>

<script>
export default {
  name: 'custom-input',
  emits: ['update:searchValue'],
  props: {
    searchValue: String,
  },
};
</script>
