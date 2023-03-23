<script lang="ts">
	import type { ImageType } from '../../types/Image';
	import Image from '../atoms/Image.svelte';

	export let image: ImageType;
	export let username: string;
</script>

<div class="user__info">
	<Image
		class="img img__profile"
		image={{
			alt: image.alt,
			src: image.src
		}}
	/>
	<h1>{username}</h1>
</div>
