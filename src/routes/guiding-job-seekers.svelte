<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/guiding-job-seekers/hero.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
</script>

<svelte:head>
	<title>Guiding job-seekers</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<img src={srcHero} class="hero rounded" alt="People standing infront of whiteboard" />
	<div class="container">
		<div class="description">
			<h1>Guiding job seekers</h1>
			<p>
				TRR works with employment transitions. They help job-seekers taking the next step in their
				careers. For example, they could help with creating a great resume and prepare you before
				your job interview.
			</p>
			<h2>Covid hits the labor market</h2>
			<p>
				In 2020 when the pandemic hit the labor market, TRR found it necessary to enable the
				job-seekers to do more independently and increase the level of self-service. TRR had a
				pre-existing portal for users. So why did we redesign it?
			</p>
			<ul>
				<li>Job-seekers didn’t find the content to be useful</li>
				<li>Bad website navigation</li>
				<li>Low use frequency</li>
				<li>Outdated content</li>
				<li>No personal approach</li>
			</ul>
			<h2>Creating guiding content</h2>
			<p>
				The amount of new job seekers at TRR was increasing every day, we were already short in time
				and our deadline was only 6 months ahead.
			</p>
			<p>
				We wanted to release something simple, yet helpful to a person who just lost their job. We
				wanted to provide the users with a basic guide to help them find a job. The idea was to
				provide them with digestible resources to enable them to take more control of their own
				journey.
			</p>
			<p>
				Me and my team with content producers and advisors at TRR accepted this challenge and our
				process ended up like the following:
			</p>
			<h3>1. Sketching the User Story</h3>
			<p>
				We started by examining the current journey for our users together with advisors from TRR
				with experience guiding job seekers. I facilitated User Story Mapping sessions with the
				advisors to sketch the journey from the point when an individual lost their job, to setting
				a goal and reaching it. TRR already had a process, but it was not common practice for all
				advisors at TRR. We needed to align the process to present it to our users which required a
				high level of collaboration.
			</p>

			<h3>2. Interview job-seekers and collect quantitative data</h3>
			<p>
				I interviewed current job-seekers about their experiences and pains during the process. Data
				from Google Analytics provided us with an understanding which content was the most popular
				in the pre-existing website. This gave us a good understanding of the biggest pain points
				during the different phases of the journey. It also provided us with a basis for
				prioritizing the most important needs to start with.
			</p>

			<h3>3. Define Jobs-to-be-done</h3>
			<p>
				For the next step, we created content in the form of text, video, and supporting images and
				illustrations. I introduced the job-to-be-done method to help us specify a customer's
				specific goal, or “job” through the process that would lead that job-seeker to “hire” a page
				to complete the job. This helped us to keep focused on what’s most important and saved us
				from a lot of unnecessary content.
			</p>

			<figure>
				<img src={srcMiro} class="box-shadow rounded" alt="Creating Jobs-to-be-done in Miro" />
				<figcaption>Creating Jobs-to-be-done in Miro.</figcaption>
			</figure>

			<h3>4. Rapidly build something</h3>
			<p>
				I created prototypes and tested them iteratively with the target group to evaluate the
				structure and the content. This made it possible for us to move fast, get feedback and
				refine. As we advanced we updated to basic web pages filled with text and placeholders for
				intended videos. We analyzed the feedback and updated the content as we gained more
				insights. We also implemented more new components like:
			</p>
			<ul>
				<li>In-page links to help the user find the content they are looking for quicker</li>
				<li>Highlighted information and tips</li>
				<li>
					Links to tie with TRR’s digital tools, to create your resume, do a personality test or
					search for jobs.
				</li>
			</ul>

			<h3>5. Guiding principles for guiding content</h3>
			<p>
				From my user tests I got a lot of insight about how users preferred to consume this type of
				content. Based on them, I created general guiding principles to help the content creators.
				Here are two examples:
			</p>
			<h4>Active words</h4>
			<p>
				The importance of using active words. The readers were generally not interested in any
				background information – they only wanted to know what to do next. For more context my
				recommendation was to provide expandable content or links to other pages with more details.
			</p>

			<h4>Keep it short and sweet</h4>
			<p>
				Use bullet lists, short and precise titles and highlighted important information to make it
				easier for the user to scan the content. Even though the original idea was to create a guide
				with connecting steps, many users didn’t start from the starting point but rather jumped
				between steps and looked for keywords. A majority of the users scanned through the pages to
				evaluate if the content were valuable to them.
			</p>
			<figure class="small">
				<img
					src={srcAnchorLinks}
					class="box-shadow rounded"
					alt="Anchor links to help readers to quickly find content"
				/>
				<figcaption>Anchor links to help readers to quickly find content</figcaption>
			</figure>

			<h2>Solution</h2>
			<p>
				We have created a guide that step-by-step describes how to create a resume and personal
				letter, how to adapt these to an application, and tips for when preparing for a job
				interview.
			</p>

			<h2>Result</h2>
			<p>
				The most important result of this project is enabling users to be independent and more in
				control of their journey to find a new job. This also resulted in a relief of workload for
				TRR's advisors who became able to focus their time on the individuals who needed personal
				support. In addition, the project has involved a new way of collaborating cross-functionally
				to create content within the organization. This has contributed to increasing the
				understanding of user-centered methods and contributed to the extended understanding of the
				user’s needs within TRR.
			</p>
		</div>

		<div class="sidebar">
			<h3>Keywords</h3>
			<li>Consumer facing</li>
			<li>Content design</li>
			<li>User Story Mapping</li>
			<li>User Test</li>
		</div>
	</div>
</section>

<style>
</style>
