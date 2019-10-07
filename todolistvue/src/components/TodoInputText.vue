<template>
  <div class="control">
    <input class="input" type="text" placeholder="Enter your tasks : " v-bind="value" />
  </div>
</template>

<script>
export default {
  props: ["value"]
};
</script>

<style>
</style>