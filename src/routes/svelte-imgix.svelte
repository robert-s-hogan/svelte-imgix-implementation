<script context="module">
	export const prerender = true;
</script>

<script>
	import Header from '$lib/header/Header.svelte'
    import imgix, { placeholder, srcset } from 'svelte-imgix';
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
                        use:imgix={"https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance"} 
                        sizes="50vw" 
                        alt="" 
                    />
					<figcaption>Picture element above the fold without lazyload</figcaption>
				</figure>
			</div>
		</div>
		<div class="intro">
			<div class="srcset">
				<h2>Img SrcSet Example #2</h2>
				<figure class="skeleton">
                    <img 
                        use:imgix={"https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance"} 
                        sizes="50vw" 
                        alt="" 
                    />
					<figcaption>Img srcset above the fold without lazyload</figcaption>
				</figure>
			</div>
		</div>
		<div class="spacer"></div>
		<div class="spacer"></div>
		<div class="lazy">
			<div class="picture">
				<h2>Non-Lazyload Img SrcSet Example #1</h2>
				<figure class="skeleton">
                    <img 
                        use:imgix={"https://vintagewineestates.imgix.net/common/images/banners/CPDawn2.jpg?auto=compress,format,enhance"} 
                        sizes="50vw" 
                        alt="" 
                    />
					<figcaption>Picture lazyloaded WITH low quality image placeholder technique</figcaption>
				</figure>
			</div>
		</div>
		<div class="lazy">
			<div class="srcset">
				<h2>Lazyload Img SrcSet</h2>
				<figure class="skeleton">
                    <img 
                        use:imgix={"https://brcohn.imgix.net/static/images/2019/03/BRCohnWinery_049_amphitheater.jpg?auto=compress,format,enhance"} 
                        sizes="50vw" 
                        alt="" 
                    />
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
	/* .skeleton::before {
        content: '';
        position: absolute;
        background: linear-gradient(
          90deg,
          transparent,
          rgba(255, 255, 255, 0.9),
          transparent
        );
        width: 50%;
        height: 100%;
        top: 0;
        left: 0;
        animation: loading 0.6s infinite;

      }

	  @keyframes loading {
        0% {
          transform: skewX(-10deg) translateX(-100%);
        }
        100% {
          transform: skewX(-10deg) translateX(200%);
        }
      } */
</style>
