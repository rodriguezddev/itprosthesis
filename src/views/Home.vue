<template>
  <div class="home">
    <Empoderamos/>
    <MisionVision/>
    <NuestrosValors/>
  </div>
</template>

<script>
// @ is an alias to /src
import Empoderamos from '@/components/Empoderamos.vue'
import MisionVision from '@/components/MisionVision.vue'
import NuestrosValors from '@/components/NuestrosValors.vue'
export default {
  name: 'Home',
  components: {
    Empoderamos,
    MisionVision,
    NuestrosValors
  }
}
</script>
