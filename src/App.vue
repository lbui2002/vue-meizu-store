<template>
  <div id="app">
    <top-bar></top-bar>
    <home-slider></home-slider>
    <site-goto></site-goto>
    <m-footer></m-footer>
  </div>
</template>

<script>
import topBar from './components/topBar'
import mFooter from './components/mfooter'
import siteGoto from './components/siteGoto'
import homeSlider from './components/homeSlider'

export default {
  components: {
    topBar,
    mFooter,
    siteGoto,
    homeSlider
  }
}
</script>

<style>
html {
  /*height: 100%;*/

}

body {
   font-family:"微软雅黑","Microsoft Yahei",Arial,Helvetica,sans-serif,"宋体";
   font-size:14px;
}
</style>
