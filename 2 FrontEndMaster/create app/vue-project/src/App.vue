<script>
import counter from './components/BaseCounter.vue'
import rondomNumbers from './components/rondomNumbers.vue'
import characterList from './components/characterList.vue'
import characterList from './components/characterListNew.vue'

  export default {
    components: {
      counter, 
      rondomNumbers,
      characterList,
      characterListNew
    },
    
  }
</script>

<template>
  <characterListNew />
  <characterList />
  <rondomNumbers />
	<counter />
</template>
