<template>
  <PicPreview :url="imageUrl" />
</template>
<script>
import PicPreview from '@/components/PicPreview'

export default {
  components: { PicPreview },

  asyncData ({ app, route, store, error }) {
    const uniqId = route.params.uniqId
    const fullUrl = `${process.env.baseUrl}pics/${uniqId}`

    return {
      imageUrl: fullUrl
    }
  },

  data: () => ({
    imageUrl: ''
  })
}
</script>
