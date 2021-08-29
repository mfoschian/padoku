<template>
	<div id="app">
		<div id="app">PadOku</div>
		<div><Cell class="cell" /></div>
	</div>
</template>

<script>
import Cell from "./components/cell.vue"


export default {
	name: "App",
	components: {
		Cell
	},
};
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}

div.cell {
	height: 100px;
	width: 100px;
}
</style>
