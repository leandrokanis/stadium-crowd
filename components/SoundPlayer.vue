<template>
  <section class="sound-player">
    <div class="player">
      <vue-audio :file="path" />
    </div>
  </section>
</template>

<script lang="js">
import VueAudio from 'vue-audio'

export default {
  name: 'SoundPlayer',

  components: {
    VueAudio
  },

  props: [],

  data () {
    return {

    }
  },

  computed: {
    path () {
      return require('~/assets/stadium1.mp3')
    }
  },

  mounted () {
  },

  methods: {
  }
}

</script>

<style scoped lang="scss">

.sound-player {

}
</style>
