<template lang="pug">
footer.footer
  .container__inner
    .footer__top
      ul.footer__list
        h3.footer__header Contact
        li
          | Twitter:
          = ' '
          a(href="https://twitter.com/vueconfus" target="_blank")
            span.at VueConf.US
        li
          | Email:
          a  hello
            span.at vueconf.us
      ul.footer__list.footer__list--small
        h3.footer__header Useful links
        //- li: nuxt-link(to="/speakers") Speakers
        //- li: nuxt-link(to="/schedule") Schedule
        li: nuxt-link(to="/workshops") Workshops
        //- li: nuxt-link(to="/terms") Terms & Conditions
        li: nuxt-link(to="/codeofconduct") Code of Conduct
        //- li: nuxt-link(to="/privacypolicy") Privacy Policy

    .footer__bottom
      //- | Proudly supported by
      //- strong  Evan You
      //- |  and
      //- a(href="https://monterail.com"): strong.footer__logo
      .footer__copyright
        | Copyright 2017-2018 ConnectEvents.io
        br
      //- .footer__legal
      //-   | Monterail.com Sp. z o.o. with its registered office in Wrocław, at 27-29 Oławska street, 50-123 Wrocław, Poland, registered with the Register of Entrepreneurs of the National Court Register maintained by the District Court of Wrocław-Fabryczna in Wrocław, VI Commercial Division of the National Court Register, under entry number KRS 0000357415, NIP [taxpayer ID] 778-147-18-20, REGON [enterprise ID] 301447685, share capital 5.000 PLN, e-mail vueconf@monterail.com.
</template>

<style lang="sass">
@import ~assets/css/base/helpers

.footer
  margin-top: 40px
  padding-top: 70px
  padding-bottom: 30px
  border-top: 1px solid #e6e6e6

.footer__top
  padding-bottom: 40px

  @media #{$medium-up}
    display: flex
    justify-content: space-around

.footer__logo
  display: inline-block
  vertical-align: middle

  &:before
    content: ''
    background-image: url('~assets/img/monterail-logotype.svg')
    margin-left: 6px
    display: inline-block
    height: 24px
    width: 119px
    background-size: contain
    background-repeat: no-repeat

.footer__list
  list-style: none
  padding: 0
  margin: 0
  font-size: 22px

  li
    line-height: 1.4
    font-weight: 300

  a
    font-weight: 400
    color: $color-link
    text-decoration: none

  &.footer__list--small
    font-size: 20px

.footer__header
  margin: 15px 0
  font-size: 36px
  font-weight: 300
  color: $color-text

.footer__bottom
  font-size: 20px
  font-weight: 400
  line-height: 36px
  text-align: center
  color: $color-text

  a
    text-decoration: none
    color: $color-text
    white-space: nowrap

.footer__img
  height: 24px
  display: inline-block
  margin-bottom: -3px
  margin-left: 4px

.footer__copyright
  font-size: 13px
  margin-top: 0
  color: #9D9D9D

.footer__legal
  font-size: 11px
  line-height: 1
  margin-top: 0
  color: #9D9D9D

span.at:before
  content: '@'
</style>
