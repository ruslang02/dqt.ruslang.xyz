<script>
	import Promo from './Promo.svelte';
	import Container from './Container.svelte';
	import Footer from './Footer.svelte';
</script>

<style>
	h2 {
		margin-bottom: 1rem;
	}
	.list {
		display: flex;
		flex-direction: column;
	}
	.list__item {
		display: flex;
		align-items: center;
		margin-bottom: 1rem;
	}
	.list__item img {
		width: 64px;
		height: 64px;
		flex-shrink: 0;
		margin-right: 1rem;
	}
</style>

<Promo />
<Container>
	<div class="block">
		<h2>
			Features
		</h2>
		<div class="list">
			<div class="list__item">
				<img alt>
				<div>
					<b>Respects your PCs resources</b>
					<div>
						Thanks to NodeGui, a project which ports Qt's GUI engine, this client does not utilize Electron or other Chromium-based technologies, which cuts RAM usage by third and CPU usage by half, all with no compromises!
					</div>
				</div>
			</div>
			<div class="list__item">
				<img alt>
				<div>
					<b>Follows Discord's style guidelines</b>
					<div>
						Unlike other clients which serve similar purpose, DiscordQt makes large emphasis on following official client's user experience guidelines, which will help you start using this client right away!
					</div>
				</div>
			</div>
			<div class="list__item">
				<img alt>
				<div>
					<b>Extras</b>
					<div>
						Although there is no such variety of plugins and themes compared to similar projects, we are actively working on implementing some of the features that are presented in other clients that could marginally improve end-user's experience (as long as it follows Discord's Terms of Service).
					</div>
				</div>
			</div>
		</div>
	</div>
</Container>
<Footer />