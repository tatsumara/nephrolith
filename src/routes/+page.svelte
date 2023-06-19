<script>
	import collection from '$lib/monsters.json'
</script>

<div class="box-container">
	{#each collection as monster}
	<h1>{monster.name}</h1>
	{/each}
</div>