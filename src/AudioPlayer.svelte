<script>
	export let audioURL = "";
	export let topic = "";
</script>


<section>
	<h6>
		Play Audio
	</h6>
	<audio controls>
		<source src={audioURL} type="audio/mp3">
		Your browser does not support the audio element.
	</audio>
</section>	


<style>
	section {
		width: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;

		margin: 0 0 20px 0;
		transition: all 1s;
	}
	
	h4 {
		margin: 5px;
	}

	audio {
		border: 1px solid black;
		padding: 10px;
		background: black;
	}
</style>