<template>
  <VueDatePicker v-model="date" inline @onChangeMonth="showConsoleMessage" />
</template>

<script>
export default {
  data: () => ({
    date: new Date()
  }),
  methods: {
    showConsoleMessage(message) {
      console.log(message);
    }
  }
};
</script>
