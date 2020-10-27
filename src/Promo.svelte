<script>
	import Container from './Container.svelte';
	import Button from './Button.svelte';
</script>

<style>
	.promo {
		background: #7289da;
		background: -moz-linear-gradient(45deg, #7289da 0%, #2a5ee8 100%);
		background: -webkit-linear-gradient(45deg, #7289da 0%,#2a5ee8 100%);
		background: linear-gradient(45deg, #7289da 0%,#2a5ee8 100%);
		filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#7289da', endColorstr='#2a5ee8',GradientType=1 );
		
		color: white;
	}
	
	.promo :global(.promo__container) {
		display: flex;
		align-items: flex-end;
	}
	
	.promo__text {
		padding: 2rem 0;
		width: 60%;
	}
	
	.promo__image {
		background-image: url(./assets/promo.png);
		background-size: cover;
		background-position: bottom center;
		width: 40%;
		min-height: 300px;
	}
	
	.promo__button-group {
		padding-top: 1rem;
	}
	
	@media (max-width: 768px) {
		.promo {
			padding: 0 1rem;
		}
		.promo :global(.promo__container) {
			display: flex;
			flex-direction: column;
			text-align: center;
		}
		.promo__text {
			width: 100%;
		}
		.promo__image {
			width: 100%;
		}
	}
	
	a {
		color: white;
		font-weight: bold;
	}
</style>

<div class="promo">
	<Container class="promo__container">
		<section class="promo__text">
			<h1>
				Best open-source client for Discord
			</h1>
			<p>
				Your favourite messaging app is now up to <b>3x faster</b> and with built-in support for <a href="#themes">themes</a> and <a href="#plugins">plugins</a>!
			</p>
			<div class="promo__button-group">
				<Button target="https://github.com/ruslang02/discord-qt/releases/latest" outline="false">
					Download
				</Button>
				<Button target="https://github.com/ruslang02/discord-qt" outline="true">
					View on GitHub
				</Button>
			</div>
		</section>
		<section class="promo__image"></section>
	</Container>
</div>