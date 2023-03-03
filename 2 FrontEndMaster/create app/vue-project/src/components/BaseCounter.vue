<script>
	export default{
		data : () => ({
			// the return here
			incrementAmount: 10,
       		count: 10,
		}),
		methods: {
			changeIncrementAmount() {
				this.incrementAmount =Number(event.target.value);
			},
			incrementCount() {
				this.count += this.incrementAmount;
			}
		} 	
	}
</script>	

<template>	
<hr>  
<div>
	<h1>counter</h1>
	<p>{{ count }}</p>
	<button v-on:click="incrementCount">increment Count</button>
	<h1>{{incrementAmount}}</h1>
	<div>
	<label for="incrementAmount"> increment by</label>
	<input
		type="number" v-model="incrementAmount"
	/>
	</div>
  </div>
</template>