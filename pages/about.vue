<template>
	<div>
		<h2>About</h2>
		<p>
			Lorem ipsum dolor sit, amet consectetur adipisicing elit. Amet optio odio
			repudiandae itaque rerum deserunt neque assumenda dolore impedit natus.
		</p>
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur nam
			at architecto sit quo in repudiandae ducimus ipsa aliquid facilis!
		</p>
	</div>
	<div>{{ data }}</div>
</template>

<script setup lang="ts">
	const { data } = await useFetch('/api/hello?name=mario', {
		method: 'post',
		body: { age: 30 },
	});
</script>

<style scoped>
	h2 {
		margin-bottom: 20px;
		font-size: 36px;
	}

	p {
		margin: 20px 0px;
	}
</style>
