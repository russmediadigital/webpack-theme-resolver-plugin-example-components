<template>
  <div style="width: 300px; left: 0; right: 0; margin: auto;">
    <list-entry
      v-for="item in items"
      :key="item.id"
      :item="item"
    />
  </div>
</template>

<script>
import ListEntry from 'awesome-components/ListEntry.vue'

export default {
  components: { ListEntry },
  props: {
    items: {
      required: true,
      type: Array
    }
  }
}
</script>
