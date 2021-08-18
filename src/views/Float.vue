<template>
	<div class="window">
		<div class="main">
			<div id="nav-clear">nav-clear</div>
			<div class="content">
				<div>asdcontent</div>
				<div>content</div>
				<div>content</div>
				<div>content</div>
			</div>
		</div>
		<div id="nav">
			nav
			<button @click="changeMenu">click</button>
		</div>
	</div>
</template>
<script>
export default {
	name: 'Float',
	methods: {
		changeMenu() {
			let nav = document.getElementById('nav');
			let navClear = document.getElementById('nav-clear');

			if (nav.style.width === '70px') {
				nav.style.width = '110px';
				navClear.style.width = '130px';
				return;
			}
			nav.style.width = '70px';
			navClear.style.width = '90px';

		}
	}
}
</script>
<style lang="scss" scoped>
@import "src/assets/scss/menu";
</style>
