<template lang="pug">
view.content
  image.logo(src="/static/logo.png")
  view.text-area
    text.title {{ title }}
</template>

<script>
export default {
  setup() {
    onShow: () => {
      console.log("222")
    }
    return {
      title: "Hello uniapp_v3",
    }
  },
}
</script>

<style lang="sass">
.content
  display: flex
  flex-direction: column
  align-items: center
  justify-content: center

.logo
  height: 200rpx
  width: 200rpx
  margin-top: 200rpx
  margin-left: auto
  margin-right: auto
  margin-bottom: 50rpx

.text-area
  display: flex
  justify-content: center

.title
  font-size: 36rpx
  color: #8f8f94
</style>
