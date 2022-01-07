<script context="module">
	export const prerender = true;
</script>

<script>
	import Header from '$lib/header/Header.svelte'
	import 'lazysizes';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<Header />
	<div class="grid">
		<div class="intro">
			<div class="picture">
				<h2>Picture Element</h2>
				<figure>
					<picture>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=640 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=640&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=640&dpr=3 3x"
						  media="(min-width: 1280w)"
						>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=512 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=512&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=512&dpr=3 3x"
						  media="(min-width: 1024w)"
						>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=374 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=374&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=374&dpr=3 3x"
						  media="(min-width: 768w)"
						>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=320 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=320&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=320&dpr=3 3x"
						  media="(min-width: 640w)"
						>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=240 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=240&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=240&dpr=3 3x"
						  media="(min-width: 480w)"
						>
						<source
						  srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=160 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=160&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=160&dpr=3 3x"
						  media="(min-width: 320w)"
						>

						<img src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640" alt="">
					  </picture>
					<figcaption>Picture element above the fold without lazyload or low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
		<div class="intro">
			<div class="srcset">
				<h2>Img SrcSet</h2>
				<figure>
					<!-- <img
						srcset="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
								https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
								https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
								https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
								https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
								https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						sizes="50vw"
						alt=""
					> -->
					<img
						srcset="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg"
						sizes="50vw"
						alt=""
					>
					<figcaption>Img srcset above the fold without lazyload or low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
		<div class="spacer"></div>
		<div class="spacer"></div>
		<div class="lazy">
			<div class="picture">
				<h2>Lazyload Picture Element</h2>
				<figure>
					<picture>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=640 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=640&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=640&dpr=3 3x"
						  media="(min-width: 1280w)"
						>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=512 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=512&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=512&dpr=3 3x"
						  media="(min-width: 1024w)"
						>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=374 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=374&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=374&dpr=3 3x"
						  media="(min-width: 768w)"
						>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=320 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=320&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=320&dpr=3 3x"
						  media="(min-width: 640w)"
						>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=240 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=240&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=240&dpr=3 3x"
						  media="(min-width: 480w)"
						>
						<source
						  data-srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=75&w=160 1x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=50&w=160&dpr=2 2x,
								  https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&q=35&w=160&dpr=3 3x"
						  media="(min-width: 320w)"
						>

						<img 
							data-src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640" 
							src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&w=640&px=16&blur=200&fm=webp"
							alt=""
							class="lazyload"
						/>
					  </picture>

					<figcaption>Picture lazyloaded WITH low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet</h2>
				<figure>
					<img
						data-srcset="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://vintagewineestates.imgix.net//static/images/2017/brands/gw/gw-wine-and-cheese-750x550.jpg?auto=compress,format,enhance&fit=crop&px=16&blur=200&fm=webp&w=320 640w"
						data-sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded WITH low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
	</div>
</section>

<style>
	.grid {
		display: grid; 
		grid-template-columns: 1fr 1fr; 
		align-items: center;
		justify-items: center;
	}
	h2 {
		text-align: center;
	}
	.spacer {
		height: 100vh;
	}
	figure {
		margin: .5rem;
	}
	img, .intro, .lazy {
		width: 100%;
	}
	figcaption {
		font-size: 80%;
	}
	.corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}
	@keyframes placeHolderShimmer{
    0%{
        background-position: -468px 0
    }
    100%{
        background-position: 468px 0
    }
}

.lazyload {
    animation-duration: 2s;
    animation-fill-mode: forwards;
    animation-iteration-count: infinite;
    animation-name: placeHolderShimmer;
    animation-timing-function: linear;
    background: #f6f7f8;
    background: linear-gradient(to right, #eeeeee 8%, #dddddd 18%, #eeeeee 33%);
    height: 96px;
    position: relative;
}
</style>
