<script>
	export default {		
		data() {			
			return {
				msg: "its work !",
				nbrList: [1, 2, 3]
			}
		}, 
	}
</script>

<template>
	<hr>
	<div>
		<h1>Random numbers</h1>
		<div>
		<!-- if else statement -->
		<p v-if="msg.length % 2 === 0"> Even : {{msg.toUpperCase()}}</p>
		<p v-else> Odd : {{msg}}</p>

		<!-- for loop -->
		<ul>
			<li v-for="nbr in nbrList">{{nbr * Math.random()}}</li>
			<li v-for="nbr of nbrList">{{nbr}}</li>
		</ul>
		</div>
	</div>
</template>