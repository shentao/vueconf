<template lang="pug">
.container
  .container__inner.post-section
    h1
      | Workshops

    speakers-list(:speakers="workshops", :adjust-img-url="true")

    .center
      nuxt-link(to="/schedule")
        button.button.speaker-button Read the workshop details
</template>

<script>
import SpeakersList from '@/components/SpeakersList'
import workshops from '@/content/speakers/workshop-list'

export default {
  components: { SpeakersList },
  data () {
    return {
      workshops
    }
  }
}
</script>

<style lang="sass" scoped>
@import ~assets/css/base/helpers

h2
  margin: 60px 0 100px

.container__inner
  text-align: center
  z-index: 2

.cfp-section
  border-top: 1px solid #ddd
  padding-top: 60px

.speaker-button
  margin-top: 30px
  margin-bottom: 40px
</style>
