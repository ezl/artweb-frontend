<template>
  <PicPreview :url="imageUrl" />
</template>
<script>
import PicPreview from '@/components/PicPreview'

export default {
  components: { PicPreview },

  asyncData ({ app, route, store, error }) {
    const uniqId = route.params.uniqId
    const fullUrl = `http://localhost:8000/pics/${uniqId}`

    return {
      imageUrl: fullUrl
    }
  },

  data: () => ({
    imageUrl: ''
  })
}
</script>
