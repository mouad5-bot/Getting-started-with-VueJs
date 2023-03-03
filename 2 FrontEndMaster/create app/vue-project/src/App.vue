<script>
  export default {
    data() {			
      return {
        incrementAmount: 10,
        count: 10,

        msg: "its work !",
        nbrList: [1, 2, 3]
      }
		},
    
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
  <div>
    <h1>project vur js</h1>
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
  <hr>
  <div>
    <h1>counter</h1>
      <p>{{ count }}</p>
      <button v-on:click="incrementCount">increment Count</button>
      <h1>{{incrementAmount}}</h1>
      <div>
        <label for="incrementAmount"> increment by</label>
        <input
          type="number"
        />
      </div>
  </div>
</template>
