<template>
  <h1 class="date">{{ now | formatDate }}</h1>
</template>

<script lang="ts">
export default {
  extends: {
    filters: {
      //   formatDate: (d: Date) => d.toLocaleTimeString(),
      formatDate: (d: Date) => d.toLocaleString(),
    },
  },
  data() {
    return {
      now: new Date(),
    }
  },
}
</script>

<style>
.date {
  color: #1e2b3a;
  padding: 10px;
}
</style>
