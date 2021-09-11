<template>
  <div id="nav">
    <config-provider>
      <router-view></router-view>
    </config-provider>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { ConfigProvider } from "ant-design-vue";
// import enUS from "ant-design-vue/es/locale/en_US";
export default defineComponent({
  name: "App",
  components: {
    ConfigProvider
  }
  // setup() {
  //   const locale : any = enUS
  //   return {
  //     locale
  //   }
  // }
})
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
