<template>
<div class="c-hand">
  <div class="c-hand__item" v-for="(item, i) in hand" :key="i">
    <CardArea
      :name="item.name"
      :src="item.src"
      :status="item.status"
      :type="item.type"
      :active="item.active"
      :x="item.x"
      :y="item.y"
      :fn="item.fn"
    />
  </div>
</div>
</template>

<script>
export default {
  props: ['hand']
}
</script>

<style lang="sass">
.c-hand
  display: flex
  width: 100%
  &__item
    width: calc(100% / 5)
</style>
