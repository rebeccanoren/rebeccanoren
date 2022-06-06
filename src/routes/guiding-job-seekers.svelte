<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/guiding-job-seekers/hero.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
</script>

<svelte:head>
	<title>TRR – Guiding job-seekers</title>
	<meta
		name="description"
		content="UX Case Study: How I used design methods to deliver results to TRR."
	/>
</svelte:head>

<section class="case">
	<div class="intro">
		<p class="xs">TRR (2020)</p>
		<h1 class="xl">Guiding job-seekers</h1>

		<p class="xs">How we created helpful and user-centered content using design methods.</p>
	</div>
	<img src={srcHero} class="rounded" alt="People standing infront of whiteboard" />

	<div class="container">
		<div class="description">
			<p class="s">
				TRR is a personal job coach. They are not looking for people to jump from job to job; they
				want to find the career that works best for you and helps you blossom into a new version of
				yourself. TRR can help you meet your goals with personalized coaching, guidance and
				training.
			</p>
			<h2 class="m">Covid hits the labor market</h2>
			<p>
				Our journey started in 2020 when the covid pandemic hit the job market. TRR realized they
				needed to enable job-seekers with more independence. They already had a pre-existing web
				application, but it had grown organically, and as a result, it was difficult to navigate.
				With more and more job-seekers relying on TRR to reach their career goals, we knew that
				redesigning the website would increase its efficacy. The other issues identified from our
				research were:
			</p>
			<ul>
				<li>Job-seekers didn’t find the content to be useful</li>
				<li>Bad website navigation</li>
				<li>Low use frequency</li>
				<li>Outdated content</li>
				<li>No personal approach</li>
			</ul>
			<h2 class="m" id="Creating-guiding-content">Creating guiding content</h2>
			<p>
				It's not easy to go through a job loss. With so much uncertainty in the air, you want to
				know what to do next and how to get back on your feet. The aim of this project was to create
				a product that helps professionals find work after losing theirs. We wanted to provide the
				users with a basic guide to help them; a guide that provides easily-digestible resources and
				enables them to take more control of their own journey. The process went like this:
			</p>

			<h3 class="s">1. Sketching the User Story ✍️</h3>
			<p>
				We started by examining the current journey for our users together with advisors from TRR
				whom have experience guiding job-seekers. I facilitated user story mapping sessions together
				with the advisors to sketch the journey from the point when an individual lost their job, to
				setting a goal and ultimately reaching it.
			</p>

			<h3 class="s">2. Research 🕵️‍♀️</h3>
			<p>
				I interviewed current job-seekers and collected quantitative data from the website itself in
				order to understand the biggest pain points during the different phases of the job-search
				process and prioritize what to start with first.
			</p>

			<h3 class="s">3. Define Jobs 💼</h3>
			<p>
				For the next step, I introduced the <a href="https://strategyn.com/jobs-to-be-done"
					>Jobs-to-be-done method</a
				>. Job-seekers hire a page to get things done. And the content acts like a tour guide to
				guide help them accomplish their goals. Through this method we were able to keep focused on
				what's most important and cut out unnecessary content.
			</p>

			<figure>
				<img src={srcMiro} class="box-shadow rounded" alt="Creating Jobs-to-be-done in Miro" />
				<figcaption class="xxs light">Creating Jobs-to-be-done in Miro.</figcaption>
			</figure>

			<h3 class="s">4. Rapidly build something 🛠</h3>
			<p>
				We needed to quickly build something to test our ideas, so we did. I made prototypes which I
				regularly tested with the target group to evaluate the structure and content. Doing so
				helped us get feedback and refine with rapid speed.
			</p>

			<h3 class="s">5. Guiding principles ⭐️</h3>
			<p>
				Based on my user tests and the results, it seemed like users didn’t tend to start from the
				very beginning when they arrived on a page. Most of them jumped around and only read parts
				of the pieces that were relevant to their current situation.
			</p>
			<p>
				They also skipped large parts; they searched for certain keywords to get an overview of what
				would be covered in further paragraphs. Therefore, I came up with guiding principles for the
				team. Here are a few examples:
			</p>
			<ul class="margin">
				<li>
					Don’t bore the audience. Use active language, and describe exactly what the reader needs
					to do next and how they can accomplish it.
				</li>
				<li>
					Provide links to additional information on other pages if necessary and make sure the
					headlines are clear and direct.
				</li>
				<li>
					Links to tie with TRR’s digital tools, to create your resume, do a personality test or
					search for jobs.
				</li>
				<li>
					Use bullet lists and highlight important information. It makes it much easier for users to
					scan the content, find what they are looking for and determine if it's valuable to them.
				</li>
			</ul>

			<h2 class="m" id="Solution">Solution</h2>
			<p>
				We have created a guide that step-by-step describes how to create a resume and personal
				letter, how to adapt these to an application, and tips for when preparing for a job
				interview. Some of the new components included:
			</p>

			<ul class="margin">
				<li>In-page links to help the user find the content they are looking for quicker.</li>
				<li>Highlighted information and tips.</li>
				<li>
					Links to tie with TRR’s digital tools, to create your resume, do a personality test or
					search for jobs.
				</li>
			</ul>

			<figure class="small">
				<img
					src={srcAnchorLinks}
					class="box-shadow rounded"
					alt="Anchor links to help readers to quickly find content"
				/>
				<figcaption class="xxs light">
					Anchor links to help readers to quickly find content
				</figcaption>
			</figure>

			<h2 class="m" id="Result">Result</h2>
			<p>
				The result of this project has been very positive in two directions: One of the greatest
				results of this project is improving the independence and control of people who struggle
				with their job search. It has resulted in a relief of workloads for TRR's advisors, who are
				now able to focus their time on the individuals who need personal support.
			</p>

			<p>
				Our second impact was a culture change at TRR. We started to collaborate across functions,
				using an agile approach to content creation. This taught the team how to use user-centered
				methods and brought non-designers closer to the users.
			</p>

			<div class="infobox rounded">
				<h2 class="m" id="About-TRR">About TRR</h2>
				<p>
					TRR is a non-profit foundation. They are working with with employment transitions and
					working life, contributing to learning and mobility within the Swedish labor market. Their
					activities are aimed at companies in the private labor market, trade union
					representatives, and company employees. <a href="https://www.trr.se/"
						>Learn more about TRR.</a
					>
				</p>
			</div>
		</div>

		<div class="sidebar">
			<div class="keywords">
				<h3 class="s">Keywords</h3>
				<ul>
					<li>Consumer facing</li>
					<li>Content design</li>
					<li>User Story Mapping</li>
					<li>User Testing</li>
				</ul>
			</div>

			<div class="Link">
				<h3 class="s">Link</h3>
				<p>Visit the <a href="https://www.trr.se/">website.</a></p>
			</div>

			<div class="navigation rounded box-shadow">
				<h5 class="xs">Contents</h5>
				<ul>
					<li><a href="#Creating-guiding-content">Creating guiding content</a></li>
					<li><a href="#Solution">Solution</a></li>
					<li><a href="#Result">Result</a></li>
					<li><a href="#About-TRR">About TRR</a></li>
				</ul>
			</div>
		</div>
	</div>
</section>

<style>
</style>
