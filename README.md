# tcg-slider

**This element is compatible with Polymer 0.5.**

__Example:__

```
	<template>
		<tcg-slider
			id="slider"
			paginationDisplayFilter="{{ paginationDisplayFilter }}"
			animationTime="{{ animationTime }}"
			treshold="{{ treshold }}"
			slides="{{ slides }}">
			<div class="slide-item s1">Content 1</div>
			<div class="slide-item s2">Content 2</div>
			<div class="slide-item s3">Content 3</div>
			<div class="slide-item s4">Content 4</div>
			<div class="slide-item s5">Content 5</div>
		</tcg-slider>
	</template>
	<script>
	Polymer({
		ready: function() {
			this.slides = this.$.slider.querySelectorAll('.slide-item');
		}
	});
	</script>
```
# Attributes

#### `slides`

Nodes of the slide item. Example: `this.$.slider.querySelectorAll('.slide-item')`

#### `paginationDisplayFilter`

Function that displays the text in each pagination item

#### `animationTime`

Milliseconds Integer

#### `treshold`

Pixel Integer for drag distance before animating to slide