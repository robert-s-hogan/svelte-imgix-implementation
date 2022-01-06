<script context="module">
	export const prerender = true;
	import 'lazysizes';
</script>

<script>
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<h1>IMGIX configuration</h1>
<div class="grid">
	<div class="intro">
		<div class="picture">
			<h2>Picture Element</h2>
			<figure>
				<img 
					src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,formatenhance&fit=crop&h=400" 
					alt=""
				/>
				<figcaption>An elephant at sunset</figcaption>
			</figure>

			<figure>
				<img 
					src="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,formatenhance&fit=crop&h=400" 
					alt=""
				/>
				<figcaption>An elephant at sunset</figcaption>
			</figure>
		</div>
		<div class="srcset">
			<h2>Img SrcSet</h2>
			<figure>
				<img 
					src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,formatenhance&fit=crop&h=400" 
					alt=""
				/>
				<figcaption>An elephant at sunset</figcaption>
			</figure>
			<figure>
				<img 
					src="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,formatenhance&fit=crop&h=400" 
					alt=""
				/>
				<figcaption>An elephant at sunset</figcaption>
			</figure>
		</div>
	</div>

	<div class="lazyload">
		<div class="picture">
			<h2>Lazyload Picture Element</h2>
			<figure>

			<img 
				src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,formatenhance&fit=crop&h=400" 
				alt=""
			/>
			<figcaption>An elephant at sunset</figcaption>
		</figure>
		<figure>

			<img 
				src="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,formatenhance&fit=crop&h=400" 
				alt=""
			/>
			<figcaption>An elephant at sunset</figcaption>
		</figure>
		</div>
		<div class="srcset">
			<h2>Lazyload Img SrcSet</h2>
			<figure>

			<img 
			src="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,formatenhance&fit=crop&h=400" 
			alt=""
			class="lazyload">
			<figcaption>An elephant at sunset</figcaption>
		</figure>
		<figure>

		<img 
			class="lazyload"
			data-src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format&fit=crop&crop=right&h=400" 
			src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format&fit=crop&crop=right&h=400&px=16&blur=200"
			alt="" />
			<figcaption>An elephant at sunset</figcaption>
		</figure>
		</div>
	</div>
</div>
</section>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat( auto-fit, minmax(400px, 1fr) );
	}

	.intro {
		height: 100vh;
	}

	h2 {
		text-align: center;
	}

	img {
		width: 100%;
		display: block;
		max-width: 400px;
	}
</style>
