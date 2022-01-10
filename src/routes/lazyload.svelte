<script context="module">
	export const prerender = true;
</script>

<script>
	import Header from '$lib/header/Header.svelte'
	import 'lazysizes';
	import Data from '$lib/Data.svelte';
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
				<figure class="skeleton">
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
				<figure class="skeleton">
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
				<h2>Lazyload Img SrcSet Lazyloaded Example #1</h2>
				<figure class="skeleton">
					<img
					srcset="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
						https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
					src="https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance&fit=crop&w=320 640w"
					sizes="50vw"
					class="lazyload"
					alt=""
				>

					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://brcohn.imgix.net/static/images/2019/03/BRCohn-7143-1.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://vintagewineestates.imgix.net/static/images/2017/brands/brc/brc-tasting-room-and-gourmet-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-2.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-6.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-4.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-3.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/vineyards-1.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/estate-5.png?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/events/cp-event-private-virutal-tasting.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/join-wine-club-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://cp.imgix.net/static/images/2019/01/home-image-1-2x.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://vintagewineestates.imgix.net/common/images/mkcknk.PNG?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
						class="lazyload"
						alt=""
					>
					<figcaption>Img srcset lazyloaded</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet Lazyloaded Example #2</h2>
				<figure class="skeleton">
					<img
						srcset="https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=640 1280w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=512 1024w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=374 768w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=320 640w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=240 480w,
							https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&crop=entropy&w=160 320w"
						src="https://vintagewineestates.imgix.net/static/images/2017/brands/cp/clos-pegase-vineyard-750x550.jpg?auto=compress,format&fit=fill?auto=compress,format,enhance&fit=crop&w=320 640w"
						sizes="50vw"
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
</style>
