<template>
  <div style="display: flex; flex-directon: row; justify-content: space-between; padding-bottom: 15px;">
    <p style="font-size: 16pt;">{{ item.title }}</p>
    <simple-button>Upvote</simple-button>
  </div>
</template>

<script>
import SimpleButton from 'awesome-components/essentials/SimpleButton.vue'

export default {
  components: { SimpleButton },
  props: {
    item: {
      required: true,
      type: Object
    }
  }
}
</script>
