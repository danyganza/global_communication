<template>
  <div>
    <div>
      <button @click="toast_notify">DELETE</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    toast_notify() {
      // Emit the custom event
      this.$root.$emit('toast_notify', { message: 'Item deleted successfully' });
    }
  }
};
</script>

<style scoped>

</style>
