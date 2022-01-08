<script context="module">
	export const prerender = true;
</script>

<script>
	import Header from '$lib/header/Header.svelte'
	import 'lazysizes';
	import Skeleton from 'svelte-skeleton'

</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<Header />
	<div class="grid">
		<div class="intro">
			<div class="picture">
				<h2>Img srcset Example #1</h2>
				<figure>
						<img
							srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
							sizes="50vw"
							alt=""
						>
					<figcaption>Picture element above the fold without lazyload</figcaption>
				</figure>
			</div>
		</div>
		<div class="intro">
			<div class="srcset">
				<h2>Img SrcSet Example #2</h2>
				<figure>
					<img
						srcset="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						sizes="50vw"
						alt=""
					>
					<figcaption>Img srcset above the fold without lazyload</figcaption>
				</figure>
			</div>
		</div>
		<div class="spacer"></div>
		<div class="spacer"></div>
		<div class="lazy">
			<div class="picture">
				<h2>Non-Lazyload Img SrcSet Example #1</h2>
				<figure>
					<img
					srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
					src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&w=320 640w"
					sizes="50vw"
					alt=""
				>

					<figcaption>Picture lazyloaded WITH low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet</h2>
				<figure>
					<img
						data-srcset="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						data-src="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&w=320 640w"
						data-sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
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
		max-width: 1280px;
		margin: 0 auto;
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
	@keyframes placeHolderShimmer{
		0%{
			background-position: -468px 0
		}
		100%{
			background-position: 468px 0
		}
	}
</style>
