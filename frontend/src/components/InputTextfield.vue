<template>
  <q-input
    outlined
    :type="type"
    :label="label"
    @change="$emit('update:modelValue', $event.target.value)"
  />
</template>

<script>
export default {
  name: "InputTextfield",
  props: {
    type: String,
    label: String,
    modelValue: String,
  }[("type", "label")],
};
</script>

<style>
</style>
