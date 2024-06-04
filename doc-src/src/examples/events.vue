<template>
  <VueDatePicker
    v-model="date"
    @onOpen="showConsoleMessage('-- datepicker opened --')"
    @onChange="showConsoleMessage('-- date changed --')"
    @onClose="showConsoleMessage('-- datepicker closed --')"
    @onDestroy="showConsoleMessage('-- datepicker destroyed --')"
    @onChangeMonth="showConsoleMessage('-- datepicker destroyed 11--')"
  />
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
