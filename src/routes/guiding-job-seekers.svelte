<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/guiding-job-seekers/hero.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
	let srcVideo = '/guiding-job-seekers/trr-tour.mov';
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
				want you to find the career that works best for you and help you blossom into a new version
				of yourself. TRR achieves this through personalized coaching, guidance and training.
			</p>
			<h2 class="m">Covid hits the labor market</h2>
			<p>
				This project with TRR started in 2020 when the Covid pandemic hit the job market. TRR
				realized they needed to enable job-seekers with more independence. They already had a
				pre-existing web application but as it had grown organically it was difficult to navigate.
				We started off with conducting user research and looked into the quantitative data to learn
				about the user needs and how the current website was performing.
			</p>

			<p>
				With more and more job-seekers relying on TRR to reach their next step in their career, we
				knew that redesigning the website would increase its efficacy. The issues identified from
				our research were:
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
				know what to do next and how to get back on your feet. The aim of this project was to guide
				job-seekers to take the next step in their careers. We wanted to provide the users with a
				basic guide to help them; a guide that provides easily-digestible resources and enables them
				to take more control of their own journey. The process went like this:
			</p>

			<h3 class="s">1. Sketching the user story from best practise ✍️</h3>
			<p>
				The first thing we did was to examine the current journey for our users together with
				advisors from TRR who have experience guiding job-seekers. I facilitated <a
					href="https://www.nngroup.com/articles/user-story-mapping/">User Story Mapping</a
				>
				sessions together with the advisors to sketch the journey from the point when an individual lost
				their job, to setting a goal and ultimately reaching it.
			</p>

			<h3 class="s">2. Interview job-seekers and collect quantitative data</h3>
			<p>
				I interviewed current job-seekers and collected quantitative data from Google Analytics in
				order to better understand the biggest pain points during the different phases of the
				job-search process. These insights were used by the team to prioritize what to start with
				first.
			</p>

			<h3 class="s">3. Define Jobs-to-be-done</h3>
			<p>
				For the next step, I introduced the <a href="https://strategyn.com/jobs-to-be-done"
					>Jobs-to-be-done method</a
				>. The method is best defined as a perspective, a lens through which you can define user
				goals. Job-seekers use our product to get a job done. In our case, examples of goals are to
				create the perfect resume or Linkedin profile. The content we created is intended to help
				them accomplish their goals. Through this method we were able to keep focused on what's most
				important and cut out unnecessary content.
			</p>

			<figure>
				<img src={srcMiro} class="box-shadow rounded" alt="Creating Jobs-to-be-done in Miro" />
				<figcaption class="xxs light">Creating Jobs-to-be-done in Miro.</figcaption>
			</figure>

			<h3 class="s">4. Rapidly build something</h3>
			<p>
				We needed to quickly build something to test our ideas, so we did. We had no ideas of
				groundbreaking interaction design in this project. Instead, our challenge was to keep the
				content relevant and easily-digestible. But also to make sure users found the right content
				to solve their tasks.
			</p>

			<p>
				As soon as we had the first drafts of content, I started to make prototypes Figma which I
				regularly tested with users. This created a feedback loop and helped us evaluate the
				structure and content with rapid speed.
			</p>

			<h3 class="s">5. Guiding principles</h3>
			<p>
				My research results indicated that users don't start reading from the beginning of page.
				Readers skim content rather than read every word.
			</p>
			<p>
				They search for certain keywords to get an overview of what is covered in the paragraph.
				With this in mind, I came up with guiding principles for the content creators in my team.
				Here are a few examples:
			</p>
			<ul class="margin">
				<li>
					Make sure headlines are clear and direct. Use bullet points and highlight important
					information.
				</li>
				<li>
					Don’t bore the audience. Use active language, describe exactly what the reader needs to do
					next and how they can accomplish it.
				</li>
				<li>
					Provide links to other pages with additional information for readers who want to learn
					more about at topic.
				</li>
			</ul>

			<h2 class="m" id="Solution">Solution</h2>
			<p>
				We have developed a step-by-step guide that describes how to create a resume and personal
				letter, how to adapt these to an application, and tips for when preparing for a job
				interview. To support a smooth skimming and reading experience, we introduced a few UI
				components in the design system:
			</p>

			<ul class="margin">
				<li>In-page links to help the user find the content they are searching for.</li>
				<li>Highlighted information and tips.</li>
				<li>
					CTAs to products behind login, to create resumes, personality tests or finding job ads.
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

			<figure>
				<video controls src={srcVideo} alt="Video showing the final product" muted>
					<track kind="captions" />
				</video>
				<figcaption class="xxs light">
					Demo of the final result and the new components. Visit the <a
						href="https://www.trr.se/uppsagd/sok-jobb/"
						>website
					</a> (only in Swedish 🇸🇪)
				</figcaption>
			</figure>

			<h2 class="m" id="Result">Result</h2>
			<p>
				The result of this project has been very positive in two directions: this project is
				improving the independence and control of people who struggle with their job search. It has
				resulted in a relief of workloads for TRR's advisors, who are now able to focus their time
				on the individuals who need personal support.
			</p>

			<p>
				The second impact was a culture change at TRR. We started to collaborate across functions,
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
					<li>Jobs-to-be-done</li>
					<li>User Story Mapping</li>
					<li>User Testing</li>
				</ul>
			</div>

			<div class="Link">
				<h3 class="s">Link</h3>
				<p>
					Visit the <a href="https://www.trr.se/uppsagd/sok-jobb/">website </a>(Only in Swedish 🇸🇪)
				</p>
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
