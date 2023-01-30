<script context="module">
	export const prerender = true;
</script>

<script>
	let srcHero = '/guiding-job-seekers/hero.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
	let srcPopcorn = '/guiding-job-seekers/popcorn-session.png';
	let srcVideo = '/guiding-job-seekers/trr-tour.mov';
	let srcDivider = 'divider.svg';
</script>

<svelte:head>
	<title>TRR – Guiding job-seekers</title>
	<meta
		name="description"
		content="UX Case Study: How I used design methods to deliver results to TRR."
	/>
</svelte:head>

<section class="case">
	<div class="container">
		<div class="description">
			<p class="xs">TRR (2020)</p>
			<h1 class="xl">Guiding job-seekers</h1>

			<p class="s">
				TRR is a personal job coach. They are not looking for people to jump from job to job; they
				want you to find the career that works best for you and help you blossom into a new version
				of yourself. TRR achieves this through personalized coaching, guidance and training.
			</p>

			<div class="summary rounded ">
				<h3>Summary</h3>
				<p>
					I was in a team of content creators producing web content to guide job seekers through the
					process to take the next step in their career. My role was to make ensure the content was
					digestable and findable by making the team empathizing with their readers.
				</p>
			</div>

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

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Creating-guiding-content">Part I: Creating Guiding Content</h2>
			<p>
				It's not easy to go through a job loss. With so much uncertainty in the air, you want to
				know what to do next and how to get back on your feet. The aim of this project was to guide
				job-seekers to take the next step in their careers. We wanted to provide the users with a
				basic guide to help them; a guide that provides easily-digestible resources and enables them
				to take more control of their own journey. The process went like this:
			</p>

			<h3 class="s">1) Sketching the User Story from Best Practise</h3>
			<p>
				The first thing we did was to examine the current journey for our users together with
				advisors from TRR who have experience guiding job-seekers. I facilitated <a
					href="https://www.nngroup.com/articles/user-story-mapping/">User Story Mapping</a
				>
				sessions together with the advisors to sketch the journey from the point when an individual lost
				their job, to setting a goal and ultimately reaching it.
			</p>
			<figure>
				<img src={srcHero} class="rounded" alt="People standing infront of whiteboard" />

				<figcaption class="xxs light">Workshop with the team and stakeholders.</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h3 class="s">2) Interview job-seekers and collect Quantitative data</h3>
			<p>
				I interviewed current job-seekers and collected quantitative data from Google Analytics in
				order to better understand the biggest pain points during the different phases of the
				job-search process. These insights were used by the team to prioritize what to start with
				first.
			</p>

			<h3 class="s">3) Define Jobs-to-be-done</h3>
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
				<figcaption class="xxs light">
					Creating Jobs-to-be-done to our User Story Map in Miro.
				</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h3 class="s">4) Rapidly build something</h3>
			<p>
				We needed to quickly build something to test our ideas, so we did. We had no ideas of
				groundbreaking interaction design in this project. Instead, our challenge was to keep the
				content relevant and easily-digestible. But also to make sure users found the right content
				to solve their tasks.
			</p>

			<p>
				As soon as we had the first drafts of content, I started to make prototypes in Figma which I
				regularly tested with users. This created a feedback loop and helped us evaluate the
				structure and content with rapid speed.
			</p>

			<figure>
				<img src={srcPopcorn} class="box-shadow rounded" alt="Collaborating in Miro" />
				<figcaption class="xxs light">
					By showing video clips and involving the team when analyzing the user tests, I was able to
					share the research findings in a fun and engaging way.
				</figcaption>
			</figure>

			<h3 class="s">5) Guiding Principles</h3>
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
					Don’t bore the audience. Use an active voice, describe exactly what the reader needs to do
					next and how they can accomplish it.
				</li>
				<li>
					Provide links to other pages with additional information for readers who want to learn
					more about at topic.
				</li>
			</ul>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Solution">Part II: Solution</h2>
			<p>
				We have developed a step-by-step guide that describes how to create a resume and personal
				letter, how to adapt these to an application, and tips for when preparing for a job
				interview. We also decided to make all the content available to the public, there is no
				longer a need for TRR users to log in every time time they want to access it. To support a
				smooth skimming and reading experience, we also introduced a few UI components in the design
				system:
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

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h2 class="m" id="Result">Part III: Result and Key Takeways</h2>
			<p>
				The result of this project has been very positive in two directions: this project is
				improving the independence and control of people who struggle with their job search. It has
				resulted in a relief of workloads for TRR's advisors, who are now able to focus on
				qualitative time with job-seekers rather than emailing PDF files and repeatedly answering
				recurring questions.
			</p>

			<p>
				The second impact was a culture change at TRR. We started to collaborate across functions,
				using an agile approach to content creation. This taught the team how to use user-centered
				methods and brought non-designers closer to the users.
			</p>

			<p>Some other things I take with me are:</p>

			<ul class="margin">
				<li>
					<strong>How to apply Jobs-to-be-done to keep focused and scope the challenge.</strong>
					<br />It was difficult for the content writers to get a hang of how to define the jobs at
					first. But once we got a hang of it in the team it was incredible effective.
				</li>

				<li>
					<strong>It's always possible to define a smaller MVP.</strong><br /> We had a difficult time
					prioritizing the content, it resulted in a large MVP and a heavy workload to have all the content
					ready before release date. Looking back, I wish we made a stricter prioritizing to increase
					the quality.
				</li>
				<li>
					<strong>The power of engaging the team in UX research.</strong> <br />I invited
					non-designer team members to participate during the user tests and analysis. This
					increased the team's intrest to act on the learnings.
				</li>
			</ul>

			<div class="infobox rounded">
				<h2 class="xs" id="About-TRR">About TRR</h2>
				<p>
					TRR is a non-profit foundation. They work with with employment transitions and working
					life, contributing to learning and mobility in the Swedish labor market. Their activities
					are aimed at companies in the private labor market, trade union representatives, and
					company employees. <a href="https://www.trr.se/">Learn more about TRR.</a>
				</p>
			</div>
		</div>

		<div class="sidebar">
			<div class="navigation rounded box-shadow blur">
				<h3>Table of contents</h3>
				<ul>
					<li><a href="#Creating-guiding-content">Part I: Creating guiding content</a></li>
					<li><a href="#Solution">Part II: Solution</a></li>
					<li><a href="#Result">Part III: Result and Key Takeways</a></li>
					<li><a href="#About-TRR">About TRR</a></li>
				</ul>
			</div>

			<div class="Link">
				<h3 class="s">Link</h3>
				<p>
					<a href="https://www.trr.se/uppsagd/sok-jobb/">Visit the website </a>(Only in Swedish 🇸🇪)
				</p>
			</div>
		</div>
	</div>
</section>

<style>
</style>
