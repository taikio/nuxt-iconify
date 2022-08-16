<template>
  <div class="container">
    <custom-buttom label="Menu" icon="menu" />
    <custom-buttom label="voltar" icon="chevron-left" />
    <custom-buttom label="Home" icon="home" />
    <custom-buttom label="Pesquisar" icon="magnify" />

    <div>
      <md-icon icon="magnify" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import CustomButtom from '@/components/CustomButton.vue'
import MdIcon from '@/components/MdIcon.vue'

export default Vue.extend({
  name: 'IndexPage',
  components: { CustomButtom, MdIcon }
})
</script>

<style scoped>
.container {
  width: 100%;
  padding: 16px 32px;
  display: flex;
  gap: 12px;
}
</style>
