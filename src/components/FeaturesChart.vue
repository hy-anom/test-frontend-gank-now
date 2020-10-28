<template>
	<div id="chart">
		<apexchart 
		type="radar" 
		height="350" 
		:options="chartOptions" 
		:series="series"
		>	
	</apexchart>
</div>
</template>

<script>
	import VueApexCharts from 'vue-apexcharts'

	export default {
		name: 'FeaturesChart',
		components: {
			apexchart: VueApexCharts,
		},
		data () {
			return {
				series: [{
					name: 'Series 1',
					data: [40, 90, 80 , 60, 40],
					enableMouseTracking: false 
				}],
				chartOptions: {
					chart: {
						height: 350,
						type: 'radar',
						toolbar: {
			      	show: false,
		      	}
					},
					xaxis: {
						categories: ['HARD SUPPORT', 'SAFE LANE', 'MID LANE', 'OFF LANE', 'SOFT SUPPORT'],
						labels: {
							style: {
	              colors: ['#5d627a','#5d627a','#5d627a','#5d627a','#5d627a'],
	              fontWeight: 600,	
	            }
						}
						
					},
					yaxis: {
						show: false,
						tickAmount: 3,
						min: 0,
						max: 100,
					},
					fill: {
						colors: ['#ED5C5E']
					},
					stroke: {
						show: true,
						width: 2,
						colors: ['#ED5C5E']
					},
					markers: {
						colors: ['#ED5C5E'],
						strokeColors: '#ED5C5E'
					},
					
					plotOptions: {
			      radar: {
			        polygons: {
								strokeWidth: 0,
								connectorColors: '#393E5E',
								fill: {
									colors: ['#36394C', '#474B64', '#5d627a']
								}
							},
			      }
			    },
					tooltip: {
						enabled: false
					}
				},
			}
		}
	}
</script>

<style lang="css" scoped>
</style>