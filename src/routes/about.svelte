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
			<p class="xs">
				I’m a Product Designer who enjoys translating thoughtful design strategies into beautiful
				and impactful experiences. 7+ years working with a range of different clients.
			</p>

			<p class="xs">
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
			<h2 class="l">It all began...</h2>
			<p>
				In high school, where my passion for design first took root. I found joy in creating
				presentations, experimenting with typography, and my favorite project of all, designing a
				newspaper magazine. In art class, I would spend hours exploring different materials,
				textures, and techniques. This allowed me to delve into a world of imagination, where
				bringing shape and color to ideas was both challenging and rewarding. I was fascinated by it
				all.
			</p>

			<p>
				Despite my art teacher's suggestion to apply to art school, I pursued studies in economics.
				However, after a year, I realized that I missed being creative. That's when I discovered the
				Bachelor program in Digital Design and Innovation created by award-winning Service Designer
				and Human-Computer Interaction researcher, <a href="http://warnestal.com/"
					>Pontus Wärnestål</a
				>. It was a game-changer for me. I had an epiphany that I could use design methodology to
				solve business problems.
			</p>

			<p>
				Combining my design training with my economics education has helped shape me into the
				designer I am today. I obsess over the details that make a design lovable, while still
				staying true to business values.
			</p>

			<h2 class="l" id="10-random-facts">10 random facts about me</h2>
			<ul class="margin">
				<li>My cat's name is Zelda, but I have never played the game.</li>
				<li>
					Favorite food: Barbecue. Nothing beats cooking food outside in fresh air and beautiful
					weather.
				</li>
				<li>
					Qualitative research is a key method in my toolbox, and I have never been in a design
					project where I haven't conducted user research. Talking to real users is my bread and
					butter.
				</li>

				<li>
					I easily become obsessed with diving into and learning new things on a regular basis. This
					sometimes worries my partner, who reminds me to eat when I'm hyper-focused.
				</li>
				<li>I've always had difficulty learning new languages. It doesn't come naturally to me.</li>
				<li>
					I've always been interested in programming. That's why I took a leave of absence in 2020
					to attend a web development boot camp for three months. I loved every second of it.
				</li>
				<li>I'm highly influenced by the Lean Startup Methodology by Eric Ries and Steve Blank.</li>
				<li>
					I have a big interest in wine. My long-term goal is to become a sommelier, but for the
					short-term, I want to attend as many wine tasting events as possible.
				</li>
				<li>
					I'm a self-proclaimed psychologist, watching reality dating shows and giving relationship
					advice to people I've never met
				</li>
				<li>If it tells you anything, I'm an ESTJ, an Executive.</li>
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

	button {
		margin-top: 40px;
	}

	@media (max-width: 1025px) {
		.container {
			justify-content: center;
			flex-direction: column;
		}

		.image {
			max-width: 400px;
		}
	}
</style>
