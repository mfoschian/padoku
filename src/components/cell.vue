<template>
	<div class="cell-notes" v-if="value == 0">
		<div v-for="i in rows" :key="i" class="row">
			<div v-for="j in cols" :key="j" class="col">
				<div class="item">{{ i }},{{ j }}</div>
			</div>
		</div>
	</div>
	<div v-else class="cell-value">
		<div class="value">
			{{ value }}
		</div>
	</div>
</template>

<script>
export default {
	props: {
		value: { type: [Number,String], default: 0 },
		notes: { type: Array, default: () => [] },
		overrides: { type: Array, default: () => [] },
		rows: { type: Number, default: 3 },
		cols: { type: Number, default: 3 },
	}
}

</script>

<style scoped>
div.cell {
	border: 1px solid black;
	background-color: beige;
	display: flex;
	flex-flow: column;
	justify-content: space-around;
}
div.row {
	/* background-color: beige; */
	display: flex;
	flex-flow: row;
	justify-content: space-around;
}
div.col {
	border: 1px solid black;
}
</style>