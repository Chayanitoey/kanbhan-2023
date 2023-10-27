<script>
	import { fade } from "svelte/transition";
</script>

<!-- center the logo -->
<div class="logo" in:fade={{ duration: 400 }} out:fade={{ duration: 400 }}>
	<picture>
		<source srcset="/svg/kanbhan_logo.svg" type="svg" />
		<img
			alt="Perfect Laundry Day Logo"
			decoding="async"
			height="100vw"
			loading="eager"
			src="/svg/kanbhan_icon.svg"
			class="logo_svg"
		/>
	</picture>
	<p class="kanbhan-logo">Kanbhan</p>
</div>

<style>
	.logo {
		margin-top: 30vh;
		display: grid;
		justify-content: center;
		opacity: 0;
	}
	.logo_svg {
		padding-left: 40%;
	}
	.kanbhan-logo {
		margin-top: 0%;
		font-family: var(--kbh-bricolage);
		font-weight: 700;
		font-size: 10vh;
		color: var(--kbh-red);
	}
</style>
