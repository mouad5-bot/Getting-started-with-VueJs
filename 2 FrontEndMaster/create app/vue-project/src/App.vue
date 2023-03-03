<script>
import counter from './components/BaseCounter.vue'
import rondomNumbers from './components/rondomNumbers.vue'

  export default {
    components: {
      counter, 
      rondomNumbers,
    },
    
  }
</script>

<template>
  <rondomNumbers />
	<counter />
	<counter />
</template>
