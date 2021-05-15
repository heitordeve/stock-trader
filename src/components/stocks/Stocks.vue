<template>
	<v-layout row wrap>
		<Stock v-for="stock in stocks" :key="stock.id" />
	</v-layout>
</template>

<script>
import Stock from './Stock'

export default {
	components: { Stock },
	data() {
		return {
			stocks: [
				{ id: 1, name: 'BMW', proce: 110 },
				{ id: 2, name: 'GOOGLE', proce: 200 },
				{ id: 3, name: 'APPLE', proce: 280 },
				{ id: 4, name: 'TWITTER', proce: 180 },
			]
		}
	}
}
</script>

<style>

</style>