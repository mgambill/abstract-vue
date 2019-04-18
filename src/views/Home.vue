<template lang="pug">
  .mt-2.text-center
    img( alt="Vue logo" src="../assets/logo.png")
    HelloWorld( msg="Welcome to Your Vue.js App" )
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue"

export default {
  name: "home",
  components: {
    HelloWorld
  }
}
</script>
