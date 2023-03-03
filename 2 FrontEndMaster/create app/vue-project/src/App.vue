<script>
import counter from './components/BaseCounter.vue'
import rondomNumbers from './components/rondomNumbers.vue'
import characterList from './components/characterList.vue'

  export default {
    components: {
      counter, 
      rondomNumbers,
      characterList,
    },
    
  }
</script>

<template>
  <characterList />
  <rondomNumbers />
	<counter />
</template>
