<script>
	import { fade } from "svelte/transition";
	import { visible } from "$lib/store/store";
</script>

<!-- center the logo -->
{#if $visible == false}
	<div
		class="flex flex-col justify-center items-center mt-60"
		in:fade={{ duration: 400 }}
		out:fade={{ duration: 400 }}
	>
		<picture>
			<source srcset="/svg/kanbhan_logo.svg" type="svg" />
			<img
				alt="Perfect Laundry Day Logo"
				decoding="async"
				height="50%"
				loading="eager"
				src="/svg/kanbhan_icon.svg"
				class="logo_svg"
			/>
		</picture>
		<h1 class="kanbhan-logo">Kanbhan</h1>
		<p class="text-md underline">Site under construction, come back later :)</p>
	</div>
{/if}

<style>
	/* .logo {
		margin-top: 30vh;
		display: block;
		justify-content: center;
		margin-left: auto;
		margin-right: auto;
		align-items: center;
	} */

	.kanbhan-logo {
		text-align: center;
		align-self: center;
		margin-top: 0%;
		font-family: var(--kbh-bricolage);
		font-weight: 700;
		font-size: 10vh;
		color: var(--kbh-red);
	}
	p {
		text-align: center;
		align-self: center;
		font-family: var(--kbh-hind);
	}
</style>
