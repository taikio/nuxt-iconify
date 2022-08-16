<template>
  <Icon :icon="computedIcon" :width="width" :height="height" :inline="true" />
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'nuxt-property-decorator'
import { Icon } from '@iconify/vue2';

@Component({
  components: { Icon }
})
export default class MdIcon extends Vue {

  @Prop({ required: true })
  icon!: string

  @Prop({ default: '1.2rem' })
  width!: string

  @Prop({ default: '' })
  height!: string

  get computedIcon () {
    return this.icon ? `mdi:${this.icon}` : ''
  }

}
</script>
