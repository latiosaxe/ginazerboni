<template>
  <section class="soon_wrapper" :class="{ 'active': active }">
    <img src="~static/logo_final.png" alt="Gina Zerboni">
    <p>Por el momento mi sitio se encuentra en construcción, pero estará listo muy pronto</p>
    <p>Si deseas ponerte en contacto conmigo puedes mandarme un correo a <a href="mailto:gina.zerboni@gmail.com">gina.zerboni@gmail.com</a>.</p>
  </section>
</template>

<script>
// import AppLogo from '~/components/AppLogo.vue'

export default {
  data () {
    return {
      active: false
    }
  },
  mounted() {
    //do something after mounting vue instance
    setTimeout(function(){
      this.active = true;
    }.bind(this), 500)
  },
  components: {
    // AppLogo
  }
}
</script>
