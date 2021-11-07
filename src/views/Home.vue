<template>
  <div class="home">
	<img alt="Vue logo" src="../assets/logo.png" />
	<div class="counter">
	  {{ counter }}
	</div>
	<div class="buttons">
	  <button class="minus" @click="decreaseCounter">-</button>
	  <button class="add" @click="increaseCounter">+</button>
	</div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
	name: "Home",
	data() {
		return {
			counter: 0,
	  	};
	},
	methods: {
		increaseCounter () {
			this.counter++;
		},
		decreaseCounter () {
			this.counter--;
		}
	}

};
</script>

<style>
div {
	margin-bottom: 0.2em;
}

.counter {
	font-size: 8em;
}

button {
	font-size: 4em;
	width: 2em;
	margin: 0 0.25em;
}

.add {
	background: green;
}

.minus {
	background: red;
}

.add:hover,
.minus:hover {
	opacity: 0.5;
}
</style>
