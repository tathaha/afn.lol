<script>
	import ArtCell from '../atoms/ArtCell.svelte';
</script>

<div class="idfk">
	<div class="contain">
		<div class="grid">
			<ArtCell art="painted_red" type="tall" />
			<ArtCell art="drowning" />
			<ArtCell art="BL1NG!" type="tall" />
			<ArtCell art="811" />
			<ArtCell art="diverge" type="tall" />
			<ArtCell art="FADE" type="tall" />
			<ArtCell art="chilly" type="tall" shrink="shrink" />
			<ArtCell art="ribbons" type="tall" />
			<ArtCell art="asumi" />
			<ArtCell art="doodle" />
		</div>
	</div>
</div>

<style>
	.grid {
		gap: 0.8rem;
		grid-auto-rows: 240px;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
	}

	.contain {
		width: min(90%, 75rem);
	}

	.idfk {
		display: flex;
		justify-content: center;
		margin-bottom: 4rem;
	}

	@media screen and (max-width: 868px) {
		.contain {
			width: min(100%, 75rem);
		}

		.grid {
			gap: 0.2rem;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			display: grid;
			grid-template-columns: 1fr 1fr 1fr;
		}
	}

	@media screen and (max-width: 600px) {
		.grid {
			grid-auto-rows: 125px;
		}
	}
</style>
