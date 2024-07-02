<script context="module">
  import { Lightbox } from 'svelte-lightbox';
</script>

<script>
  let userJourney = {
    img: '/sinch/onboarding/user-journey.svg',
    imgMobile: '/sinch/onboarding/user-journey.png',
    desc: 'The main phases when testing Sinch SMS API',
  };

  let time = {
    img: '/sinch/onboarding/time.svg',
    imgMobile: '/sinch/onboarding/time.png',
    desc: 'I conducted a detailed analysis of the tests, measuring the time each participant spent on the tasks.',
  };

  let oldDesign = {
    img: '/sinch/onboarding/old-design.svg',
    imgMobile: '/sinch/onboarding/old-design.png',
    desc: 'Previous design of the Getting started page before improvements',
  };

  let docs = {
    img: '/sinch/onboarding/docs.png',
    desc: 'Getting started section in SMS API Documentation',
  };

  let error = {
    img: '/sinch/onboarding/error.png',
    desc: 'An improved suggestion would be: "In test mode, the SMS API only sends messages to verified phone numbers. This ensures security. Verify your number in the Sinch Customer Dashboard."',
  };

  let motivation = {
    img: '/sinch/onboarding/motivation.svg',
    imgMobile: '/sinch/onboarding/motivation.png',
    desc: 'Illustration showing where developers drop off in the onboarding funnel',
  };

  let parameters = {
    img: '/sinch/onboarding/parameters.svg',
    imgMobile: '/sinch/onboarding/parameters.png',
    desc: 'All parameters in one place',
  };

  let input = {
    img: '/sinch/onboarding/input.svg',
    imgMobile: '/sinch/onboarding/input.png',
    desc: 'Added the functionality to verify a new number directly on this page, eliminating the need for users to navigate to another page which was the case before.',
  };

  let apiResponse = {
    img: '/sinch/onboarding/API-response.svg',
    imgMobile: '/sinch/onboarding/API-response.png',
    desc: 'A link to message logs and the API response was added to give more details to developers',
  };

  let selectLanguage = {
    img: '/sinch/onboarding/select-language.gif',
    desc: 'Users can now select their preferred language to access documentation',
  };

  let newPage = {
    img: '/sinch/onboarding/new-page.svg',
    imgMobile: '/sinch/onboarding/new-page.png',
    desc: 'New design of the SMS Getting started page after the improvements',
  };

  let optimalJourney = {
    img: '/sinch/onboarding/optimal-journey.svg',
    imgMobile: '/sinch/onboarding/optimal-journey.png',
    desc: 'Our goal was to streamline the SMS API onboarding, reducing completion time to under 5 minutes',
  };

  let competitorResearch = {
    img: '/sinch/onboarding/competitor-research.svg',
    imgMobile: '/sinch/onboarding/competitor-research.png',
    desc: 'I mapped the onboarding journeys of all major competitors. Here is one example.',
  };

  let competitors = {
    img: '/sinch/onboarding/competitors.svg',
    imgMobile: '/sinch/onboarding/competitors.png',
    desc: 'Comparison of competitors',
  };

  let srcVideo = '/sinch/onboarding/API-key.mov';

  let srcDivider = 'divider.svg';

  let srcSinch = '/sinch/vision/sinch.svg';

  let enter1 = false;
</script>

<style>
</style>

<svelte:head>
  <title>Developers Getting started with Sinch SMS AP</title>
  <meta
    name="description"
    content="Developers Getting started with Sinch SMS API"
  />
</svelte:head>

<section class="case">
  <div class="container">
    <div class="description">
      <p class="xs">Sinch (2024)</p>
      <h1 class="xl">Developers getting started with Sinch SMS API</h1>
      <p class="s">
        As Sinch adopts a Product-Led Growth (PLG) strategy, optimizing the user
        experience for developers integrating our SMS API is a priority. To
        enhance conversion rates, I led our newly established Onboarding Team to
        streamline the journey for new sign-ups, enabling them to quickly start
        using the SMS API and convert into paying customers.
      </p>

      <div class="summary rounded">
        <p>Summary</p>
        <p>
          As the UX Design Lead, I led my team to enhance the onboarding
          experience for Sinch's SMS API. I conducted user tests to identify
          pain points, and with an agile approach, we made significant
          improvements. We streamlined the process by making API parameters
          easier to locate, enhancing documentation, and adding better error
          handling. These changes reduced the time to the "Aha-moment,"
          resulting in a smoother and more reliable experience. As a result,
          user satisfaction and conversion rates increased. This is an ongoing
          project.
        </p>
      </div>

      <h2 class="m" id="Part1">
        Part I: What is the current onboarding experience like?
      </h2>

      <p>
        After sign up, users needed to find the option "SMS" and "Getting
        Started" in the menu. In this page users could send test messages,
        explore links to documentation and learn about a few benefits about
        upgrading.
      </p>

      <div class="lightbox">
        <Lightbox description="{oldDesign.desc}">
          <picture>
            <source srcset="{oldDesign.imgMobile}" media="(max-width: 600px)" />
            <source srcset="{oldDesign.img}" media="(min-width: 601px)" />
            <img
              src="{oldDesign.img}"
              alt="{oldDesign.desc}"
              class="box-shadow rounded"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{oldDesign.desc}</p>
      </div>

      <p>
        Another crucial resource when using the SMS API is the documentation. It
        offers step-by-step guidance and detailed explanations to ensure a
        smooth integration process. The "Getting Started" section is
        specifically tailored for new users, with guides and SDKs available in
        multiple programming languages, allowing users to find resources in
        their preferred language.
      </p>

      <div class="lightbox">
        <Lightbox description="{docs.desc}">
          <picture>
            <img
              src="{docs.img}"
              alt="{docs.desc}"
              class="box-shadow rounded"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{docs.desc}</p>
      </div>

      <h3>Sending a test SMS</h3>
      <p>
        I began by examining the current experience. I conducted user tests with
        10 backend and full-stack developers of varying experience levels. These
        developers were tasked with using our SMS API to build a small
        application and send a test SMS to themselves using their code editor.
        By doing this, we could examine the entire journey and identify
        potential problems firsthand. This method allowed us to:
      </p>

      <ul class="margin">
        <li>
          <b>Observing developers in a natural setting:</b> using their own code
          editors provided insights into how our API is utilized in real-world scenarios.
        </li>
        <li>
          <b>Directly witnessing the challenges and frustrations</b> developers faced
          helped us pinpoint specific areas that needed improvement.
        </li>
        <li>
          <b>Developers provided immediate, candid feedback</b> about their experience,
          enabling us to understand their perspectives and needs better.
        </li>
        <li>
          <b
            >Assess how effectively our documentation and support resources
            assisted</b
          > developers in overcoming obstacles.
        </li>
      </ul>

      <p>The user test covered these phases of product experience:</p>

      <div class="lightbox">
        <Lightbox description="{userJourney.desc}">
          <picture>
            <source
              srcset="{userJourney.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{userJourney.img}" media="(min-width: 601px)" />
            <img src="{userJourney.img}" alt="{userJourney.desc}" />
          </picture>
        </Lightbox>
        <p class="image-description">{userJourney.desc}</p>
      </div>

      <h2>Key research insights</h2>
      <p>
        We found that only 3 out of the 10 participants successfully sent an SMS
        to themselves, which was below our expectations. Our goal was to achieve
        a 100% success rate, with each participant completing the process within
        5 minutes. To understand the reasons behind this outcome, we examined
        the entire user journey of each participant.
      </p>

      <div class="lightbox">
        <Lightbox description="{time.desc}">
          <picture>
            <source srcset="{time.imgMobile}" media="(max-width: 600px)" />
            <source srcset="{time.img}" media="(min-width: 601px)" />
            <img src="{time.img}" alt="{time.desc}" />
          </picture>
        </Lightbox>
        <p class="image-description">{time.desc}</p>
      </div>

      <p>
        From the analysis, the pain points detected during the process were;
        Difficult to find the right section in documentation, difficult to find
        the parameters in the platform and lack of error handling.
      </p>
      <h3>Difficult to find the right section in documentation</h3>
      <p>
        Some participants struggled to find the correct section for their
        preferred language in our documentation, with two spending 16 and 25
        minutes respectively. This difficulty was primarily due to broken and
        confusing links on the platform, making it challenging for them to
        navigate to the appropriate section. However, once they found the right
        section in the documentation, it only took them a couple of minutes to
        understand what they needed to do.
      </p>

      <h3>Difficult to find the parameters in the platform</h3>
      <p>
        To use the Sinch SMS API, participants needed to navigate the platform
        to locate three parameters: 1) their API token, 2) Service Plan ID, and
        3) the Sinch test number provided for the trial. Most participants used
        links from the documentation to find them. However, they encountered
        several challenges in the process and still struggled to navigate the
        platform to find these three parameters. It took, on average, 6-8
        minutes for the participants to locate them.
      </p>

      <figure>
        <video
          controls
          src="{srcVideo}"
          alt="Video showing the final product"
          muted
        >
          <track kind="captions" />
        </video>
        <figcaption class="xxs light">
          A participant explains the struggle to locate parameters
        </figcaption>
      </figure>

      <h3>Lack of error handling</h3>

      <p>
        Due to fraud attacks on our platform, some regions are temporarily
        restricted from sending SMS. Unfortunately, this means users in these
        regions aren't able to try the SMS API either. During the user test, UK
        numbers were blocked. Participants simply didn't receive an SMS and they
        were not informed about it. This created uncertainty about their
        verified phone numbers, leading some to think they had entered the wrong
        number upon registration. As a result, participants thought they made a
        mistake and therefore tried to change the number which the SMS should be
        sent to, which led to another error. The API responded with "Messages
        can only be sent to your verified number in test mode." Users didn't
        understand what "in test mode" meant.
      </p>

      <p>
        The lack of clear communication and transparency breaks trust.
        Participants felt uncertain and frustrated, doubting the reliability of
        the platform. They questioned whether their actions were correct and
        whether the service was dependable. The eroded confidence in the API and
        the platform as a whole makes them less likely to trust and use the
        service in the future.
      </p>

      <div class="lightbox">
        <Lightbox description="{error.desc}">
          <picture>
            <img
              src="{error.img}"
              alt="{error.desc}"
              class="box-shadow rounded"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{error.desc}</p>
      </div>

      <div class="divider">
        <img src="{srcDivider}" alt="Divider svg" />
      </div>
      <h2 class="m" id="Part2">
        Part II: How might we ensure all participants are successful in sending
        a test SMS within 5 minutes?
      </h2>
      <p>
        To reiterate, ensuring all participants can build an app and send a test
        SMS within 5 minutes is vital. It shows the Sinch SMS API is easy and
        reliable, creating a strong first impression. Developers have low
        motivation at the start and need quick proof that it works. If it fails,
        they will quickly abandon it. A smooth first experience builds trust,
        leading to more conversions.
      </p>

      <div class="lightbox">
        <Lightbox description="{motivation.desc}">
          <picture>
            <source
              srcset="{motivation.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{motivation.img}" media="(min-width: 601px)" />
            <img src="{motivation.img}" alt="{motivation.desc}" />
          </picture>
        </Lightbox>
        <p class="image-description">{motivation.desc}</p>
      </div>

      <h3>Benchmarking & setting goals</h3>
      <p>
        I conducted a competitor analysis to compare our onboarding experience
        with that of our main competitors. The goal was to understand how our
        experience measures up, recognizing that developers often evaluate
        multiple providers before making a decision. This involved benchmarking
        their onboarding processes against ours, focusing on key aspects:
      </p>

      <ul>
        <li>
          How users were guided through the first encounter with the SMS API
        </li>
        <li>How important concepts like test numbers were explained</li>
        <li>The clarity and accessibility of documentation</li>
        <li>
          The availability and quality of tutorial videos or interactive guides
        </li>
        <li>The effectiveness of the UI</li>
      </ul>
      <p>
        By examining how competitors structured their onboarding journeys, what
        support materials they provided, and how they guided new users, we
        gained valuable insights into industry best practices.
      </p>

      <div class="lightbox">
        <Lightbox description="{competitorResearch.desc}">
          <picture>
            <source
              srcset="{competitorResearch.imgMobile}"
              media="(max-width: 600px)"
            />
            <source
              srcset="{competitorResearch.img}"
              media="(min-width: 601px)"
            />
            <img
              src="{competitorResearch.img}"
              alt="{competitorResearch.desc}"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{competitorResearch.desc}</p>
      </div>

      <p>
        The comparative analysis highlighted our strengths and pinpointed areas
        where we lagged behind. It helped identify specific improvements we
        could make to streamline our process, reduce friction, and enhance the
        overall user experience. Leveraging these insights allowed us to align
        our onboarding process more closely with industry standards and best
        practices, ultimately making it more competitive and appealing to
        developers.
      </p>

      <div class="lightbox">
        <Lightbox description="{competitors.desc}">
          <picture>
            <source
              srcset="{competitors.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{competitors.img}" media="(min-width: 601px)" />
            <img src="{competitors.img}" alt="{competitors.desc}" />
          </picture>
        </Lightbox>
        <p class="image-description">{competitors.desc}</p>
      </div>

      <p>
        Fueled by insights from competitor analysis and the user tests, we set
        clear goals to address the biggest challenges in our onboarding process.
        Our primary objective was to remove roadblocks and ensure a smooth,
        competitive experience for developers We systematically tackled these
        issues by working in fast iterations. Focusing on eliminating friction
        and optimizing the onboarding funnel, and optimize the onboarding funnel
        for a smoother and more developer-friendly experience.
      </p>

      <h3>Goal 1: Reduce API Errors & help users solve them if they occur</h3>
      <p>
        To keep the API stable and reliable, we regularly checked logs and
        listened to user feedback to fix problems. I users weren't able to send
        SMS we made sure to inform users. This helped maintain trust by keeping
        users aware of any issues affecting message delivery.
      </p>

      <h4>Analytics & help users solve errors</h4>
      <p>
        Users lacked sufficient information about issues, so we added a link to
        our analytics tool, Message Search, when the API request was sent.
        Message Search provides detailed SMS logs, including error code
        descriptions, timestamps, delivery status, and fees. This allows users
        to understand and resolve issues related to the API request and
        increases the discoverability of Message Search. Long term, we plan to
        display this data directly in the UI on this page, but that is a later
        milestone.
      </p>

      <p>
        Additionally, we added the API response directly in the UI because we
        noticed some participants were using the browser console to view it.
        This change ensures users can easily access important information
        without resorting to technical workarounds.
      </p>
      <div class="lightbox">
        <Lightbox description="{apiResponse.desc}">
          <picture>
            <source
              srcset="{apiResponse.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{apiResponse.img}" media="(min-width: 601px)" />
            <img src="{apiResponse.img}" alt="{apiResponse.desc}" />
          </picture>
        </Lightbox>
      </div>

      <h3>Goal 2: Reduce time to find parameters</h3>
      <p>
        Users were spending too much time searching for parameters, hindering
        the overall efficiency of their journey. They needed to navigate through
        multiple sections to retrieve them, often getting lost in the process.
        To address this, we aimed to keep them on the same page by consolidating
        all necessary parameters in one location.
      </p>
      <div class="lightbox">
        <Lightbox description="{parameters.desc}">
          <picture>
            <source
              srcset="{parameters.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{parameters.img}" media="(min-width: 601px)" />
            <img src="{parameters.img}" alt="{parameters.desc}" />
          </picture>
        </Lightbox>
      </div>

      <h3>Goal 3: Shorten time to find right section in documentation</h3>
      <p>
        To reduce the risk of having users struggle to find the right section in
        the documentation, we reviewed all critical links in the documentation
        and platform to ensure they functioned properly. We collaborated closely
        with the documentation team, suggesting improvements to help users find
        the right sections more quickly.
      </p>

      <p>
        We also introduced a dropdown with all SDKs and Rest API guides
        available. This was to help users faster find the most suitable section
        in the documentation.
      </p>

      <div class="lightbox">
        <Lightbox description="{selectLanguage.desc}">
          <picture>
            <img
              src="{selectLanguage.img}"
              alt="{selectLanguage.desc}"
              class="box-shadow rounded"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{selectLanguage.desc}</p>
      </div>

      <h3>Goal 4: Prevent errors</h3>
      <p>
        Users testing the SMS API can only send messages to phone numbers
        verified on their account to prevent fraud and ensure platform security.
        Previously, the input field allowed users to type in numbers, causing
        errors when unverified numbers were entered. To reduce these errors and
        improve user experience, we replaced the input field with a dropdown
        menu of verified numbers.
      </p>

      <p>
        We also added the functionality to verify a new number directly on this
        page, eliminating the need for users to navigate to another page which
        was the case before.
      </p>
      <div class="lightbox">
        <Lightbox description="{input.desc}">
          <picture>
            <source srcset="{input.imgMobile}" media="(max-width: 600px)" />
            <source srcset="{input.img}" media="(min-width: 601px)" />
            <img src="{input.img}" alt="{input.desc}" />
          </picture>
        </Lightbox>
      </div>

      <div class="divider">
        <img src="{srcDivider}" alt="Divider svg" />
      </div>

      <h2 class="m" id="Result">Result</h2>
      <p>
        The goal of this project was to optimize the onboarding journey for new
        developers testing the SMS API using an agile approach. We identified
        numerous user pain points and tracked the time it took for users to try
        the SMS API, aiming to reduce this time to under 5 minutes. My team and
        I enhanced the UI of the SMS Getting Started page and collaborated with
        other teams to improve the backend, API functionality, documentation,
        and test number provisioning.
      </p>

      <div class="lightbox">
        <Lightbox description="{optimalJourney.desc}">
          <picture>
            <source
              srcset="{optimalJourney.imgMobile}"
              media="(max-width: 600px)"
            />
            <source srcset="{optimalJourney.img}" media="(min-width: 601px)" />
            <img src="{optimalJourney.img}" alt="{optimalJourney.desc}" />
          </picture>
        </Lightbox>
        <p class="image-description">{optimalJourney.desc}</p>
      </div>

      <p>
        This ongoing project will be evaluated by usability tests in August
        2024. However, we have already observed a surge in conversion rates and
        other metrics such as increased user satisfaction, reduced onboarding
        time, and higher engagement levels.
      </p>

      <p>
        Looking ahead, we will continue optimizing the SMS onboarding journey.
        Our focus will expand to cover more steps of the product adoption
        journey, including introducing messaging logs and providing better
        guidance on selecting phone numbers for sending live messages.
      </p>

      <div class="lightbox">
        <Lightbox description="{newPage.desc}">
          <picture>
            <source srcset="{newPage.imgMobile}" media="(max-width: 600px)" />
            <source srcset="{newPage.img}" media="(min-width: 601px)" />
            <img
              src="{newPage.img}"
              alt="{newPage.desc}"
              class="box-shadow rounded"
            />
          </picture>
        </Lightbox>
        <p class="image-description">{newPage.desc}</p>
      </div>

      <div class="infobox rounded" id="About-Sinch">
        <p>About Sinch</p>
        <p>
          Sinch provides communication APIs and applications for smooth
          interaction between companies and their customers. Their solutions
          cover diverse communication channels including SMS, voice, video, and
          social media platforms. This enables businesses to effectively engage
          with their audience across multiple platforms and devices, ensuring
          enhanced connectivity and customer satisfaction. <a
            href="https://www.sinch.com/">Learn more about Sinch.</a
          >
        </p>
      </div>

      <div class="next-case">
        <h3>Next up</h3>
        <a data-sveltekit-prefetch href="/sinch-vision">
          <figure
            on:mouseenter="{() => {
              enter1 = !enter1;
            }}"
            on:mouseleave="{() => {
              enter1 = false;
            }}"
            class="item"
          >
            <img
              src="{srcSinch}"
              class="box-shadow border rounded-XL"
              alt="Design of Sinch Vision"
            />
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
          <li><a href="#Part1">Part I: Current onboarding experience</a></li>
          <li>
            <a href="#Part2"
              >Part II: How might we ensure all participants are successful in
              sending a test SMS within 5 minutes?
            </a>
          </li>
          <li><a href="#Result">Result</a></li>
          <li><a href="#About-Sinch">About Sinch</a></li>
        </ul>
      </div>
    </div>
  </div>
</section>
