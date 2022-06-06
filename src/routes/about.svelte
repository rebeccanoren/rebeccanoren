<script context="module">
	export const prerender = true;
</script>

<script>
	let srcRebecca = '/rebecca.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
</script>

<svelte:head>
	<title>About Rebecca – Product Designer</title>
	<meta
		name="description"
		content="I’m a Product Designer who enjoys translating thoughtful design strategies into beautiful and impactful experiences. 5+ years working with a range of different clients."
	/>
</svelte:head>

<section class="about">
	<div class="container">
		<div class="description">
			<h1 class="xl">Hey, I'm Rebecca.</h1>
			<p class="s">
				I’m a Product Designer who enjoys translating thoughtful design strategies into beautiful
				and impactful experiences. 5+ years working with a range of different clients.
			</p>

			<p class="s">
				Except for doing design, I’m currently into quantitative data analysis, improving my coding
				skills and growing knowledge about wine (but not at the same time).
			</p>
			<a href="#10-random-facts"><button>10 random facts about me</button></a>
		</div>
		<div class="image">
			<img src={srcRebecca} class="rounded" alt="Rebecca" />
		</div>
	</div>

	<div class="container">
		<div class="description">
			<h2 class="l">It all started...</h2>
			<p>
				When I was in high school. What I enjoyed the most was creating presentations, experimenting
				with typography and my favorite project: creating the design for a news paper magazine. In
				art class, I spent hours exploring the materials, textures and techniques. It took me to a
				world of imagination – giving shape and colors to what is in your mind is challenging and
				equally rewarding, all of it fascinated me.
			</p>

			<p>
				When my art teacher suggested that I apply to art school, I never considered it as a valid
				career path. Instead, I persued studies in economics. It was great, but after one year I
				missed being creative. I discovered the Bachelor program <a
					href="https://www.hh.se/utbildning/program/digital-design-och-innovation.html"
					>Digital Design and Innovation</a
				>, created by <a href="http://warnestal.com/">Pontus Wärnestål</a> – an award-winning Service
				Designer and Human-Computer Interaction researcher. I applied and got in. I had an aha-moment
				when I realized that I could design methodology to solve business problems. The rest is history.
			</p>

			<p>
				My design training in combination with my studies in economics has shaped me into the
				designer I am today. I’m obsessed with details that makes a design lovable but I don’t drift
				away from the business values.
			</p>

			<h2 class="l" id="10-random-facts">10 random facts about me</h2>
			<ul class="margin">
				<li>My cat’s name is Zelda, but I have never played the game.</li>
				<li>
					Favorite food: Barbecue. Nothing beats cooking food outside in fresh air and beautiful
					weather.
				</li>
				<li>I believe the best ideas are the simplest.</li>

				<li>
					I get easily obsessed with diving into and learning things on a regular basis. This
					sometimes worries my partner who reminds me to eat when I’m in hyper-focused.
				</li>
				<li>
					I’ve always had difficult times learning new languages, it doesn’t come naturally to me.
				</li>
				<li>
					I’ve always been interested in programming. That’s why I took a leave of absence in 2020
					to attend a web development boot camp for 3 months. I loved every second of it.
				</li>
				<li>I’m highly influenced by the Lean Startup Methodology by Eric Ries and Steve Blank.</li>
				<li>
					I have a big interest in wine, my long-term goal is to become a sommelier. For the
					short-term: Attending to as many wine tasting events as possible.
				</li>
				<li>
					I’m a self-proclaimed psychologist watching reality dating shows and giving relationship
					advice to people I’ve never met.
				</li>
				<li>If it tells you anything I’m an ESTJ, an Executive.</li>
			</ul>
		</div>
	</div>
</section>

<style>
	.container {
		justify-content: center;
		align-items: center;
	}

	.image img {
		max-width: 100%;
		width: 100%;
	}

	@media (max-width: 1025px) {
		.container {
			justify-content: center;
			flex-direction: column;
		}

		.image {
			background-color: red;
			max-width: 400px;
		}
	}
</style>
