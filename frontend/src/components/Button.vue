<template>
  <q-btn :label="label" :type="type" :color="color" class="float-right" />
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    type: String,
    label: String,
    color: String,
  },
};
</script>

<style scoped>
</style>
