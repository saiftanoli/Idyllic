<template>
  <div id="app">
    <nav-bar></nav-bar>
    <idyllic-transform></idyllic-transform>
    <idyllic-about></idyllic-about>
    <pic-gallery></pic-gallery>
    <idyllic-footer></idyllic-footer>
  </div>
</template>

<script>
import NavBar from "./components/navBar.vue";
import IdyllicTransform from "@/components/idyllicTransform.vue";
import IdyllicAbout from "@/components/idyllicAbout.vue";
import PicGallery from "@/components/picGallery.vue";
import IdyllicFooter from "@/components/IdyllicFooter.vue";
export default {
  components: {
    NavBar,
    IdyllicTransform,
    IdyllicAbout,
    PicGallery,
    IdyllicFooter,
  },
};
</script>
