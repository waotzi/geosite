<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>Geocats - Game</title>
	<meta name="description" content="A Retro-style 2D Action Platformer - Our adventure story takes the player through the world of GeoTerra, a place of both breathtaking beauty and chilling dystopian environments." />
</svelte:head>

<div id="game" class="black">
	<div class="content">
	<iframe frameborder="0" src="https://itch.io/embed-upload/5627461?color=000000" allowfullscreen="" width="640" height="480"><a href="https://nonaco.itch.io/geocats">Play Geocats on itch.io</a></iframe>
	</div>

</div>
<section>
	<center>
	<iframe frameborder="0" src="https://itch.io/embed/1484216?bg_color=0d0f15&amp;fg_color=d9d737&amp;link_color=b933a2&amp;border_color=333333" width="552" height="167"><a href="https://nonaco.itch.io/geocats">Geocats by Nonaco</a></iframe>

	</center>
</section>
<style>
	.black {
		background-color: black;
		height: 110vh;
		margin-top: 12rem;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;

	}
	.content {
		background-color: black;
		width: 100%;
		margin: auto;
		text-align: center;
		max-width: 760px;
	}
	section {
		margin-bottom: 10rem;
	}

</style>
