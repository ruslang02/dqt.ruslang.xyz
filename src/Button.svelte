<script>
	export let target = "#";
	export let outline = "false";
	function isOutline() {
		return outline === "true";
	}
</script>

<style>
	a {
		padding: .4rem 1rem;
		border: 3px solid white;
		background: white;
		color: #5769a6;
		border-radius: .25rem;
		box-shadow: 0 2px 10px rgba(0, 0, 0, 0.15);
		font-weight: bold;
		font-size: 18px;
		margin-right: .5rem;
	}
	a.outline {
		color: white;
		background: none;
	}
</style>

<a href={target} class={isOutline() ? "outline" : ""}><slot></slot></a>