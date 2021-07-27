<template>
  <div class="repository__title">
    <slot name="repTitle"></slot>
  </div>
  <div class="repository__text">
    <slot name="repText"></slot>
  </div>
  <div class="repository__state">
    <slot name="repState"></slot>
  </div>
</template>
<script>
import { repository } from '../../components/repository'

export default {
  name: 'repository',
  components:{
    repository
  }

}
</script>
<style lang="scss" scoped>

</style>