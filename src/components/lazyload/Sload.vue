<template>
	<div>
		<div v-if="loadding">加载中。。。</div>
		<slot v-else :data="data"></slot>
	</div>
</template>

<script>
	export default {
		name: "Sload",
		props: ['url'],
		data() {
			return {
				loadding: true,
				data: {}
			}
		},
		created() {
			setTimeout(() => {
				this.loadding = false;
				this.data = {
					name: 'zhangbin'
				};
			}, 2000);
		}
	}
</script>

<style scoped>

</style>
