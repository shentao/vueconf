<template lang="pug">
.section.post-section.cfp-section
  .cfp-video
    iframe(
      width="520"
      height="292"
      src="https://www.youtube.com/embed/i9SK-l2gQEE?rel=0&amp;showinfo=0"
      frameborder="0"
      allowfullscreen
    )
  .cfp-content
    h1 Join the band!
    h4 Call for Papers Open Now

    p We're looking for submissions on all things Vue.js!

    .center
      nuxt-link(to="/schedule")
        button.button.speaker-button Apply as a speaker
  //- .nav-target#apply
  //- .center
  //-   include:markdown-it ../content/speakers/cfp.md

  //-   a.post-section__button.button(href="https://docs.google.com/forms/d/e/1FAIpQLSdtbxBpV0j_zCnELXQuIkeGH8x6gaOWE0J8tTsAdpa0O5MYOw/viewform" target="_blank")
  //-     | Apply as a speaker

  //-   p.post-section__paragraph
  //-     | We will come back to you within a few days.
</template>

<script>
export default {
}
</script>

<style lang="sass" scoped>
@import ~assets/css/base/helpers

.speaker-button
  margin: 40px 0 10px

.cfp-video
  display: inline-block
  max-width: 100%
  vertical-align: middle
  text-align: left

  @media #{$medium-up}
    padding: 0 20px 0 0
    max-width: calc(60% - 40px)

.cfp-content
  display: inline-block
  max-width: 100%
  vertical-align: middle
  text-align: left

  @media #{$medium-up}
    padding: 0 20px
    max-width: calc(40% - 40px)

  h1, h4
    margin: 0

</style>
