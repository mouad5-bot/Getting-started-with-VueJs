<template>
	<h1>links</h1>
		  <div>
			<a
			  :href="github"
			>
			github 
			</a> <br>
			<a
			  :href="twitter"
			>
			  twitter
			</a>
		  </div>
  </template>

<script>
export default {
	name: "headerBerLinks",
	data (){
		return{
		github : "https://github.com/mouad5-bot",
		twitter : "https://twitter.com/FifelMouad"

		}
	}
}
</script>