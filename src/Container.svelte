<style>
	.container {
		margin: 0 auto;
		width: 100%;
		display: flex;
	}

	@media (min-width: 576px) {
		.container {
			width: 512px;
		}
	}

	@media (min-width: 768px) {
		.container {
			width: 704px;
		}
	}

	@media (min-width: 992px) {
		.container {
			width: 928px;
		}
	}
</style>
<div class="container {$$props.class}">
	<slot></slot>
</div>