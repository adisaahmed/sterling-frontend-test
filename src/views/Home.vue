<template>
	<div id="app">
		<AllData v-bind:alldatas="alldatas" />
		<b-container>
			<b-row>
				<b-col>1 of 3</b-col>
				<b-col>1 of 3</b-col>
				<b-col>1 of 3</b-col>
			</b-row>
		</b-container>
	</div>
</template>

<script>
	import AllData from '../components/AllData';
	import axios from "axios";

	export default {
		name: 'Home',
		components: {
			AllData
		},

		data() {
			return {
				alldatas: []
			}
		},

		methods: {

		},

		created() {
			axios.get("https://swapi.co/api/people?")
			.then(res => this.alldatas  = res.data)
		}
	}
</script>