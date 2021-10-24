<template lang="html">
  <div>
    <p>{{ bar }}</p>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export const FooBar = Vue.extend({
  computed: {
    bar: function (): string {
      return this.foo;
    },
  },
  data: function () {
    return {
      foo: "bar",
    };
  },
});

export default FooBar;
</script>
