<script>
	import collection from '$lib/monsters.json'
</script>

<div class="box-container">
	{#each collection as monster}
		<div class="box">
			<h1>{monster.name}</h1>
			{#if monster.collection}
				<p>{monster.collection}</p>
			{/if}
			{#if monster.tags}
				{#each monster.tags as tag}
					<p>{tag}</p>
				{/each}
			{/if}
		</div>
	{/each}
</div>