<script>
	import { page } from '$app/stores';

	$('#slider').on('input change', (e) => {
		const sliderPos = e.target.value;
		// Update the width of the foreground image
		$('.foreground-img').css('width', `${sliderPos}%`);
		// Update the position of the slider button
		$('.slider-button').css('left', `calc(${sliderPos}% - 18px)`);
	});
</script>

<body>
	<div class="container">
		<div class="img background-img" />
		<div class="img foreground-img" />
		<input type="range" min="1" max="100" value="50" class="slider" name="slider" id="slider" />
		<div class="slider-button" />
	</div>
</body>

<style>
</style>
