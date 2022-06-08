<script setup>
import { defineComponent, ref } from 'vue';
import { isYesterday, addDays } from 'date-fns/esm';

const onPanelChange = () => {
  alert(`On panel change Triggered!!`);
};
</script>

<template>
  <n-calendar #="{ year, month, date }" :on-panel-change="onPanelChange">
    {{ year }}-{{ month }}-{{ date }}
  </n-calendar>
</template>
