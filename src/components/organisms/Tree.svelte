<script lang="ts">
	import LinkList from '../molecules/LinkList.svelte';
	import UserInfo from '../molecules/UserInfo.svelte';
	import type { LinkType } from '../../types/Link';

	const links: LinkType[] = [
		{
			href: 'https://twitch.tv/aleezito',
			image: {
				alt: 'twitch',
				src: '/twitch.png'
			},
			text: 'Twitch'
		},
		{
			href: 'https://instagram.com/aleezito',
			image: {
				alt: 'instagram',
				src: '/instagram.png'
			},
			text: 'Instagram'
		},
		{
			href: 'https://www.tiktok.com/@aleezito_',
			image: {
				alt: 'tiktok',
				src: '/tiktok.png'
			},
			text: 'Tiktok'
		},
		{
			href: 'https://www.twitter.com/aleezito_',
			image: {
				alt: 'twitter',
				src: '/twitter.png'
			},
			text: 'Twitter'
		},
		{
			href: 'https://www.youtube.com/@aleezito',
			image: {
				alt: 'youtube',
				src: '/youtube.png'
			},
			text: 'Youtube'
		}
	];
</script>

<div class="tree">
	<UserInfo
		username="Aleezito"
		image={{
			alt: 'profile',
			src: '/user.png'
		}}
	/>
	<LinkList {links} />
</div>
