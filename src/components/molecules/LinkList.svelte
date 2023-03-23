<script lang="ts">
	import type { LinkType } from '../../types/Link';
	import Link from './Link.svelte';

	export let links: LinkType[];
</script>

<ul class="list">
	{#each links as item}
		<Link {item} />
	{/each}
</ul>
