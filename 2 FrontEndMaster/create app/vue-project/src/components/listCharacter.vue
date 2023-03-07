<script>
	export default {		
		data: () => ({	
			listCharacter: [
				{
					name : "animals",
					element : ["dog", "cat", "monkey"]
				},
				{
					name : "first",
					element : ["dog"]
				},
				{
					name : "second",
					element : ["cat"]
				},
				{
					name : "theird",
					element : ["monkey"]
				}
			],
			favoriteCharacter: [],	
		}),
		methods: {
			favoriteCharacter(character) {
				this.favoriteCharacter.push(character);
			}
		}
	}
</script>

<template>
	<hr>
	<div>
		<h2>characters New</h2>
		<p v-if="listCharacter.length === 0"> There are no character</p>
		<ul v-else-if="listCharacter.length % 2 === 0">
			<li v-for="(character, index) in listCharacter" :key="`even-charcter-${index}`">
				<p>{{ character.neme }}</p>
				<button @click="favoriteCharacter(character)"> $%*! favorite</button>
			</li>
		</ul>
		<p v-else> There are odd characters!</p>
	</div>
</template>