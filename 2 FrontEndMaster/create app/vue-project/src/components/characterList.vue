<script>
	export default{
		data: () => 
		({
			characters:[
				// {
				// 	name : 'mouad'
				// },
				// {
				// 	name : 'khalid'
				// },
				// {
				// 	name : 'UsF'
				// }
			]
		})  
	} 
</script>

<template>	
	<div>
		<h1>Names</h1>
		<div id="app">
			<!-- if else statement -->
			<p v-if="characters.length === 0"> Opss !! There are no characters </p>
			<p v-else> 
				<ul>
					<li v-for="character in characters">{{ character.name }}</li>
				</ul>
			</p>
		</div>
	</div>
</template>