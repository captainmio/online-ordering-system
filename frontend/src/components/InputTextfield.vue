<template>
  <q-input outlined :type="type" v-model="text" :label="label" />
</template>

<script>
export default {
  name: "InputTextfield",
  props: ["type", "label"],
};
</script>

<style>
</style>
