<script lang="ts">
	import type { LinkType } from '../../types/Link';
	import Image from '../atoms/Image.svelte';

	export let item: LinkType;
</script>

<li class="link">
	<a href={item.href} target="_blank">
		<Image class="img img__link" image={item.image} />
		<span>{item.text}</span>
	</a>
</li>
