<script lang="ts">
	import type { ImageType } from '../../types/Image';

	let clazz: string;
	export { clazz as class };
	export let image: ImageType;
</script>

<img class={clazz} src={image.src} alt={image.alt} />
