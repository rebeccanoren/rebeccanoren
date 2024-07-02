<!-- <script context="module">
	export const prerender = true;
</script> -->

<script>
	let srcHero = '/guiding-job-seekers/hero.jpg';
	let srcAnchorLinks = '/guiding-job-seekers/anchor-links.png';
	let srcMiro = '/guiding-job-seekers/miro.jpg';
	let srcPopcorn = '/guiding-job-seekers/popcorn-session.png';
	let srcVideo = '/guiding-job-seekers/trr-tour.mov';
	let srcDivider = 'divider.svg';
	let userjourney = '/guiding-job-seekers/jobbsokarprocess.png';

	let srcSinch = '/sinch/vision/sinch.svg';
	let enter1 = false;
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
			<p class="xxs">TRR (2020)</p>
			<h1 class="xl">Empowering job-seekers</h1>

			<p class="xs">
				TRR is a personalized job coaching service that helps individuals find their ideal career
				path and supports them in their professional development. Rather than encouraging
				job-hopping, TRR aims to enable people to flourish in their chosen careers through
				personalized coaching, guidance, and training.
			</p>

			<div class="summary rounded ">
				<p>Summary</p>
				<p>
					As a UX Designer working with a team of content creators, my role was to ensure that the
					website content was easily digestible and accessible for job-seekers. I facilitated the
					design process and made sure the team empathized with their readers to make the content
					more relatable.
				</p>
			</div>

			<h2 class="m">Impact of COVID-19 on the Labor Market</h2>
			<p>
				The TRR project began in 2020 when the COVID-19 pandemic caused significant upheaval in the
				job market. TRR recognized that job-seekers needed more independence and support, and
				although they had an existing website, it had grown organically, making it difficult to
				navigate. I started off with conducting user research to learn more. We interviewd 5
				job-seekers about their struggles.
			</p>
			<p>The issues identified from the research were:</p>
			<ul>
				<li>Job-seekers didn’t find the website to be useful</li>
				<li>Difficult to find what they were looking for</li>
				<li>Lack of a personalized approach</li>
				<li>Outdated content</li>
				<li>Low use frequency</li>
			</ul>
			<p>
				The obvious solution based on our time constraints was to provide with readable content to
				guide users trough the job-seeking process. Allowing job-seekers to take the steps at their
				own pace would also improve the quality of the 1-1 meetings with advisors.
			</p>

			<p>
				We analyzed quantitative data to understand user needs and evaluate the website's
				performance. Job-seekers were typically directed to relevant pages by their advisors, and we
				used the number of page views as an indicator of the content's significance.
			</p>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>
			<h2 class="m" id="Creating-guiding-content">Part I: Creating Guiding Content</h2>
			<p>
				Losing a job can be a daunting experience, especially in times of uncertainty. The objective
				of our project was to provide job-seekers with a basic guide that would assist them in
				taking the next step in their career by offering easily-digestible resources and empowering
				them to take control of their journey. Here's how we achieved that:
			</p>

			<h3 class="s">1) Sketching the User Story from Best Practise</h3>
			<p>
				To begin, we used <a href="https://www.nngroup.com/articles/user-story-mapping/"
					>User Story Mapping</a
				> as a method and collaborated with TRR advisors who had experience guiding job-seekers. Together,
				we examined the current journey of users and mapped out the journey from the point when an individual
				loses their job to setting a goal and achieving it. We also highlighted the pain points of the
				job-seekers during different stages of their journey.
			</p>
			<figure>
				<img src={userjourney} class="" alt="Creating Jobs-to-be-done in Miro" />
				<figcaption class="xxs light">The user journey to find a job</figcaption>
			</figure>

			<div class="divider">
				<img src={srcDivider} alt="Divider svg" />
			</div>

			<h3 class="s">2) Interview job-seekers and collect quantitative data</h3>
			<p>
				To gain a better understanding of the major pain points during the various phases of
				job-search process, I conducted interviews with current job-seekers and collected
				quantitative data from Google Analytics. The insights I gathered were used by the team to
				prioritize their approach and determine which content to focus on first.
			</p>

			<figure>
				<img src={srcHero} class="rounded" alt="People standing infront of whiteboard" />

				<figcaption class="xxs light">Workshop with the team and stakeholders.</figcaption>
			</figure>

			<h3 class="s">3) Define Jobs-to-be-done</h3>
			<p>
				In the following step, I introduced the <a href="https://strategyn.com/jobs-to-be-done"
					>Jobs-to-be-done method</a
				> to guide our content creation process. This approach allows us to define user goals and identify
				what job-seekers are trying to accomplish when using our product. By understanding their goals,
				such as creating the perfect resume or LinkedIn profile, we were able to create content that
				is tailored to their needs. This framework helped us stay focused on the most critical content
				and eliminate any unnecessary information.
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
					Bullet points break down complex concepts into manageable segments, making information
					easier to comprehend. Highlighting key takeaways and critical points draws readers'
					attention to the most important information. These techniques create a more accessible and
					engaging reading experience.
				</li>
				<li>
					Utilize an active voice and provide precise instructions on what the reader should do next
					to progress in their job search. Clarify the next step in their journey and guide them
					through the process of accomplishing it. This approach will keep your audience focused and
					motivated towards achieving their employment goals.
				</li>
				<li>
					Including links to additional resources is a helpful practice for providing readers with
					more comprehensive information on a topic. By adding relevant links, readers who want to
					delve deeper into a subject can access more detailed resources.
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

			<div class="infobox rounded" id="About-TRR">
				<p>About TRR</p>
				<p>
					TRR is a non-profit foundation. They work with with employment transitions and working
					life, contributing to learning and mobility in the Swedish labor market. Their activities
					are aimed at companies in the private labor market, trade union representatives, and
					company employees. <a href="https://www.trr.se/">Learn more about TRR.</a>
				</p>
			</div>

			<div class="next-case">
				<h3>Next up</h3>
				<a data-sveltekit-prefetch href="/sinch-vision">
					<figure
						on:mouseenter={() => {
							enter1 = !enter1;
						}}
						on:mouseleave={() => {
							enter1 = false;
						}}
						class="item"
					>
						<img src={srcSinch} class="box-shadow border rounded-XL" alt="Design of Sinch Vision" />
						<figcaption>
							<p class="uppercase xxs">Sinch (2024)</p>
							<h3 class="l nomargin {enter1 ? 'underline' : ''}">
								Ongoing work: Improve the process to buy phone numbers
							</h3>
							<div class="tags">
								<span>Design Strategy</span> <span>User Research</span>
							</div>
						</figcaption>
					</figure>
				</a>
			</div>
		</div>

		<div class="sidebar">
			<div class="navigation rounded box-shadow blur">
				<p>Table of contents</p>
				<ul>
					<li><a href="#Creating-guiding-content">Part I: Creating guiding content</a></li>
					<li><a href="#Solution">Part II: Solution</a></li>
					<li><a href="#Result">Part III: Result and Key Takeways</a></li>
					<li><a href="#About-TRR">About TRR</a></li>
				</ul>
			</div>


		</div>
	</div>
</section>

<style>
</style>
