<script>
import counter from './components/BaseCounter.vue'
import rondomNumbers from './components/rondomNumbers.vue'
import characterList from './components/characterList.vue'
import listCharacter from './components/listCharacter.vue'
import barLinks from './components/header-bar-links.vue'

  export default {
    components: {
      barLinks,
      counter, 
      rondomNumbers,
      characterList,
      listCharacter,
    },
    data: () => ({
      newCharacter : {
        name : "",
        element: [],
      },
			favoriteList: [],	
    }),
    
  }
</script>

<template>
  <barLinks />
  <listCharacter />
  <characterList />
  <rondomNumbers />
	<counter />
</template>
