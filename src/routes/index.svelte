<script context="module">
	export const prerender = true;
</script>

<script>
	import Counter from '$lib/Counter.svelte';
	import assetImg from '$lib/assets/image.png';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<h1>
		<div>
			<img src="image.png" alt="static/image.png" />
		</div>
		<div>
			<img src="{assetImg}" alt="src/lib/assets/image.png" />
		</div>
	</h1>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}
</style>
