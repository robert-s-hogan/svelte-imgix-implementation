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
				<h2>Example #1</h2>
				<figure class="skeleton">
						<img
							srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
									https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
							sizes="50vw"
							class="skeleton"
							alt=""
						>
					<figcaption>above the fold img</figcaption>
				</figure>
			</div>
		</div>
		<div class="intro">
			<div class="srcset">
				<h2>Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
								https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						sizes="50vw"
						class="skeleton"
						alt=""
					>
					<figcaption>above the fold img</figcaption>
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
	.skeleton:empty {
		cursor: progress; 
		width: 160px;
		height: 107px;
		background: 
			linear-gradient(0.25turn, transparent, #fff, transparent),
			linear-gradient(#eee, #eee),
			radial-gradient(38px circle at 19px 19px, #eee 50%, transparent 51%),
			linear-gradient(#eee, #eee);  
		background-repeat: no-repeat;
		border: 2px solid #efefef;
		animation: skeleLoading 1.5s infinite;
	}
	@media(min-width: 480px) {
		.skeleton:empty {
			width: 240px;		
			height: 164px;
		}
	}
	@media(min-width: 640px) {
		.skeleton:empty {
			width: 320px;	
			height: 217px;	
		}
	}
	@media(min-width: 768px) {
		.skeleton:empty {
			width: 374px;		
			height: 253px;
		}
	}
	@media(min-width: 1024px) {
		.skeleton:empty {
			width: 512px;		
			height: 345px;
		}
	}
	@media(min-width: 1280px) {
		.skeleton:empty {
			width: 640px;	
			height: 431px;	
		}
	}

	
	@keyframes skeleLoading {  
		to {
			background-position: 315px 0, 0 0, 0 190px, 50px 195px;
		}
	}
</style>
