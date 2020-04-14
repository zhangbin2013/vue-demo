<template>
	<div class="about">
		<h1>This is an about page</h1>
		<layout>
			<!-- v-slot:header 简写 #header -->
			<template #header>头部</template>
			<template v-slot:default>
				<s-lay></s-lay>
			</template>
			<template v-slot:footer>尾部</template>
		</layout>
	</div>
</template>
<script>
	import Layout from '@/views/Layout';
	import SLay from '@/components/lazyload/SLay';

	export default {
		name: 'About',
		components: { SLay, Layout }
	};
</script>
