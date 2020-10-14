<template>
<div class="c-field">
  <div class="c-field__item" v-for="(item, i) in field" :key="i">
    <CardArea
      :name="item.name"
      :src="item.src"
      :status="item.status"
      :active="item.active"
      :type="item.type"
    />
  </div>
</div>
</template>

<script>
export default {
  props: ['field'],
  mounted(){
  }
}
</script>

<style lang="sass">
.c-field
  display: flex
  width: 100%
  &__item
    width: calc(100% / 5)
</style>
