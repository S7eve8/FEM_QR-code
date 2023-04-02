<script setup>
defineProps({
	imagePath: {
		type: String,
		required: true
	},
	title: {
		type: String,
		required: true
	},
	message: {
		type: String,
		required: true
	}
})
</script>

<template>
	<div class="qr-con flex flex-col rounded-2xl p-3.5">
		<div>
			<img class="rounded-2xl" :src="imagePath" alt="qr code image" />
		</div>
		<div class="flex flex-col items-center gap-2 p-5 text-center">
			<p class="dark-blue text-xl font-bold">{{ title }}</p>
			<p class="grayish-blue text-md leading-5">{{ message }}</p>
		</div>
	</div>
</template>

<style scoped>
.qr-con {
	background-color: var(--white);
}
</style>
