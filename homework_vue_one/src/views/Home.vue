<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!--  <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" /> -->
    <app-header> </app-header>
    <div class="test">
      <rv> </rv>
      <sidebar> </sidebar>
    </div>
    <appFooter> </appFooter>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
/* import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src */
import appHeader from "@/components/appHeader.vue";
import rv from "@/components/rv.vue";
import sidebar from "@/components/sidebar.vue";
import appFooter from "@/components/appFooter.vue";

@Component({
  components: {
    /* HelloWorld, */
    appHeader,
    rv,
    sidebar,
    appFooter,
  },
})
export default class Home extends Vue {}
</script>

<style>
.test {
  display: flex;
  min-height: calc(100vh - 360px);
  margin-bottom: 15px;
  
}
.home{
  min-height: 100vh;
}

</style>
