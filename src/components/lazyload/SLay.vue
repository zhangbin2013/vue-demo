<template>
	<div>
		<sload url="http://baidu.com" #default="{data}">
			<div>我来欢迎你{{data.name}}</div>
		</sload>
	</div>
</template>

<script>
	import Sload from './Sload';

	export default {
		name: 'SLay',
		components: {
			Sload
		}
	};
</script>

<style scoped>

</style>
