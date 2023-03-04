<script>
	export default {		
		data: () => ({	
			characterListNew: [
				{
					name : "car",
					element : ["res", "bleu", "white"]
				},
				{
					name : "animal",
					element : ["dog", "cat", "monky"]
				},
				{
					name : "country",
					element : ["morocco", "franch", "usa"]
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
		<p v-if="characterListNew.length === 0"> There are no character</p>
		<ul v-else-if="characterListNew.length % 2 === 0">
			<li v-for="(character, index) in characterListNew" :key="`even-charcter-${index}`">
				<p>{{ character.neme }}</p>
				<button @click="favoriteCharacter(character)"> $%*! favorite</button>
			</li>
		</ul>
		<p v-else> There are odd characters!</p>
	</div>
</template>