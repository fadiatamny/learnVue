<template>
  <div>
    <div>
      <h3 @click="$emit('test')">{{ data.title }}</h3>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  name: "Todo",
  props: ["data"],
  data: function() {
    return {};
  },
  methods: {
  }
});
</script>

<style></style>
