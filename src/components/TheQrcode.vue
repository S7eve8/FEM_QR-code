<script setup>
import AttributionComp from './AttributionComp.vue'
import QrCode from './QrCodeComp.vue'
import QrCodeImagePath from '@/assets/images/image-qr-code.png'
</script>

<template>
	<div class="relative flex h-full items-center justify-center">
		<QrCode
			class="qr-comp"
			:imagePath="QrCodeImagePath"
			title="Improve your front-end skills by building projects"
			message="Scan the QR code to visit Frontend Mentor and take your coding skills to the next level"
		>
		</QrCode>
		<AttributionComp
			attributorName="8teve"
			attributorLink="https://www.frontendmentor.io/profile/S7eve8"
			class="absolute bottom-0"
		></AttributionComp>
	</div>
</template>

<style scoped>
.qr-comp {
	max-width: 335px;
}
</style>
