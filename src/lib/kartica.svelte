<script lang="ts">
	import type { Opis } from './types';
	export let opis: Opis;
	const { name, image, description } = opis;
</script>

<div class=" bg-gray-600 flex flex-col items-center p-5 rounded-2xl">
	<h3 class="text-white">{name.toUpperCase()}</h3>
	<!-- svelte-ignore a11y-missing-attribute -->
	<img class="w-1/1.5 rounded-2xl" src={image} />
	<p class="p-5 my-3 bg-gray-400 rounded-xl">
		{description}
	</p>
	<a
		href="https://sl.wikipedia.org/wiki/Glavna_stran"
		class="bg-slate-700 hover:bg-slate-800 text-white p-3 rounded-xl">Preberi več</a
	>
</div>
