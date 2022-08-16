<template>
  <button type="button">
    <md-icon v-if="icon" :icon="icon" width="1.2rem" />
    {{ label }}
  </button>
</template>

<script lang="ts">
import Vue from 'vue'
import MdIcon from '@/components/MdIcon.vue'

export default Vue.extend({
  components: { MdIcon },
  props: {
    label: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      default: ''
    }
  }
})
</script>

<style scoped>
button {
  outline: none;
  padding: 6px 12px;
  border: 1px solid #cecee4;
  border-radius: 6px;
  background: transparent;
  color: aqua;
  font-weight: 600;
  display: flex;
  align-items: center;
}
</style>
