<script context="module">
	export const prerender = true;
</script>

<script>
	let srcGuidingJobSeekers = '/guiding-job-seekers/guding-job-seekers.png';
	let srcFindingTalent = '/finding-talent/finding-talent.png';
	let srcMeetings = '/book-meetings/book-meetings.png';
	let srcSinch = '/sinch/sinch.png';

	let enter1 = false;
	let enter2 = false;
</script>

<svelte:head>
	<title>Rebecca Norén – Product Designer</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
<section class="intro">
	<h1 class="xl">
		I'm a strategic & hands-on Product Designer. Based in France, working globally.
	</h1>
	<p>My works are just a scroll away.</p>
</section>

<section class="works">
	<div class="works-grid">
		<a sveltekit:prefetch href="/guiding-job-seekers">
			<figure
				on:mouseenter={() => {
					enter1 = !enter1;
				}}
				on:mouseleave={() => {
					enter1 = false;
				}}
				class="item"
			>
				<img
					src={srcGuidingJobSeekers}
					class="box-shadow"
					alt="Guiding content showing text and a video."
				/>
				<figcaption>
					<p class="uppercase xxs">TRR (2020)</p>
					<h3 class="l nomargin {enter1 ? 'underline' : ''}">Guiding job-seekers</h3>
					<p>A new experience to enable job-seekers to take the next step in their career.</p>
					<div class="tags">
						<div><span>JTBD</span> <span>User Story Mapping</span> <span>User Test</span></div>
					</div>
				</figcaption>
			</figure>
		</a>

		<a sveltekit:prefetch href="/matching-employers-job-seekers">
			<figure
				on:mouseenter={() => {
					enter2 = !enter2;
				}}
				on:mouseleave={() => {
					enter2 = false;
				}}
				class="item"
			>
				<img src={srcFindingTalent} class="" alt="Searching tool to find candidates to recruit" />
				<figcaption>
					<p class="uppercase xxs">TRR (2019)</p>
					<h3 class="l nomargin {enter2 ? 'underline' : ''}">
						Matching employers with job-seekers
					</h3>
					<p>
						Unlocking customer value by identifying and acting on opportunities and refining ideas.
					</p>
					<div class="tags">
						<span>User Research</span> <span>Impact Mapping</span> <span>Design Sprint</span>
					</div>
				</figcaption>
			</figure>
		</a>

		<figure class="item">
			<img src={srcMeetings} class="" alt="Screenshot of Insights in Miro" />
			<figcaption>
				<p class="uppercase xxs ">TRR (2021)</p>
				<h3 class="l  nomargin">Defining a best practice for meetings</h3>
				<p>Performing interviews and analysis to learn.</p>
				<div class="tags">
					<span>User Research</span>
				</div>
			</figcaption>
		</figure>

		<figure class="item">
			<img src={srcSinch} class="" alt="Design of Sinch Vision" />
			<figcaption>
				<p class="uppercase xxs">Sinch (2023)</p>
				<h3 class="l nomargin {enter2 ? 'underline' : ''}">Redesigning the Sinch Platform</h3>
				<div class="tags">
					<span>Design Strategy</span> <span>User research</span> <span>SaaS</span>
				</div>
			</figcaption>
		</figure>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: left;
		flex: 1;
	}

	figure {
		width: 100%;
	}

	.works {
		padding: 32px;
	}

	.works a {
		color: var(--text-color);
	}

	.works-grid {
		display: flex;
		flex-direction: column;
		flex: auto;
		width: 100%;
		gap: 200px;
	}

	.works-grid .item {
		display: flex;
		gap: 48px;
		justify-content: left;
		flex-direction: row;
		padding: 0px;
		margin: 0px;
		width: 100%;
		transition: transform 0.2s;
	}

	img {
		max-width: 500px;
		border-radius: 20px;
		object-fit: fill;
		box-shadow: 0px 0px 0px 0px rgba(53, 7, 69, 0.1), 0px 9px 19px 0px rgba(53, 7, 69, 0.1),
			-2px 34px 34px 0px rgba(53, 7, 69, 0.06), -4px 77px 46px 0px rgba(53, 7, 69, 0.1),
			-6px 136px 54px 0px rgba(53, 7, 69, 0.02), -10px 213px 60px 0px rgba(53, 7, 69, 0.05);
	}

	.intro {
		margin-top: 100px;
	}

	.intro h1 {
		max-width: 100%;
	}

	figcaption {
		margin: 0;
		display: flex;
		flex-direction: column;
		justify-content: center;
		text-align: left;
		min-width: 350px;
	}

	figcaption h3 {
		margin-top: 10px;
	}

	.tags {
		margin: 28px 0;
		display: flex;
		flex-wrap: wrap;
		gap: 12px;
	}

	span {
		background-color: var(--light-blue);
		color: var(--accent-color);
		padding: 8px 16px;
		border-radius: 8px;
		font-size: 14px;
		white-space: nowrap;
		box-shadow: 0 15px 30px 0 rgb(0 42 102 / 4%), inset 1px 1px 1px 0 hsl(0deg 0% 100% / 90%);
	}

	a:hover {
		text-decoration: none;
	}

	.underline {
		text-decoration: underline;
	}

	/* Animations */
	.works-grid .item:hover {
		transform: scale(0.95);
		text-decoration: none;
	}

	/* Media Queries */

	@media (max-width: 1025px) {
		.works-grid {
			flex-direction: column;
			align-items: center;
			gap: 100px;
		}

		.works-grid .item {
			flex-direction: column;
			align-content: center;
		}

		figure {
			display: flex;
			align-items: center;
		}

		img {
			max-width: 90%;
			border-radius: 15px;
		}

		span {
			font-size: 12px;
		}
	}
</style>
