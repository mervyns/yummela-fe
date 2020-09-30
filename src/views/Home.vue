<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <auth-modal/>
  </div>
</template>

<script>
// import { mapState,mapMutations } from 'vuex'
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import AuthModal from '@/components/Modals/AuthModal.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    AuthModal
  },
  // computed: mapState({
  //   showModal: state => state.showAuthModal
  // }),
  // methods: {
  //   ...mapMutations({
  //     showAuthModal: "showAuthModal",
  //     hideAuthModal: "hideAuthModal"
  //   }),
  // }
}
</script>