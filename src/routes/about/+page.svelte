<script context="module">
</script>

<script>
  let srcRebecca = '/rebecca.jpg';
  let srcRebeccaFlowers = '/rebecca-flowers.jpg';
</script>

<style>
  .about .container {
    padding: 0 40px;
  }
  .container {
    justify-content: center;
    align-items: center;
    margin-top: 0px;
  }

  .container .description {
    padding: 0 16px;
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
      max-width: 350px;
    }
  }
</style>

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
        I’m a Product Designer who enjoys translating thoughtful design
        strategies into beautiful and impactful experiences. 7+ years working
        with a range of different clients.
      </p>

      <p class="xs">
        Except for doing design, I’m currently into quantitative data analysis,
        improving my coding skills and growing knowledge about wine (but not at
        the same time).
      </p>
      <a href="#10-random-facts"><button>10 random facts about me</button></a>
    </div>
    <div class="image">
      <img src="{srcRebeccaFlowers}" class="rounded-XL" alt="Rebecca" />
    </div>
  </div>

  <div class="container">
    <div class="description">
      <h2 class="l">About me</h2>
      <p>
        Hi there! I'm a UX designer with a deep-rooted passion for creativity
        that sparked in high school. I found joy in creating presentations,
        experimenting with typography, and my favorite project was designing a
        newspaper magazine. Art class was where I thrived, exploring various
        materials and techniques, turning ideas into vibrant realities.
      </p>

      <p>
        Although I initially pursued economics, I quickly realized that my heart
        was set on creativity. Discovering the Bachelor program in Digital
        Design and Innovation was a turning point. This program, led by
        award-winning Service Designer Pontus Wärnestål, opened my eyes to the
        powerful intersection of design and business. I learned how to use
        design methodology to solve complex business problems, and it ignited my
        passion for combining creativity with practicality.
      </p>

      <p>
        Today, I bring together my design skills and economics background to
        create user-centered designs that are both visually appealing and highly
        functional. I focus on the small details that make a design truly
        special, always striving to deliver work that brings joy and value. I'm
        committed to creating designs that not only look great but also solve
        real user needs and align with business goals. I'm excited to bring my
        passion for design and my analytical mindset to every project.
      </p>

      <h2 class="l" id="10-random-facts">10 random facts about me</h2>
      <ul class="margin">
        <li>
          Favorite food: Barbecue. Nothing beats cooking food outside in fresh
          air and beautiful weather.
        </li>
        <li>
          Qualitative research is a key method in my toolbox, and I have never
          been in a design project where I haven't conducted user research.
          Talking to real users is my bread and butter.
        </li>

        <li>
          I easily become obsessed with diving into and learning new things on a
          regular basis. This sometimes worries my partner, who reminds me to
          eat when I'm hyper-focused.
        </li>
        <li>
          I've always had difficulty learning new languages. It doesn't come
          naturally to me.
        </li>
        <li>
          I've always been interested in programming. That's why I took a leave
          of absence in 2020 to attend a web development boot camp for three
          months. I loved every second of it.
        </li>
        <li>
          I'm highly influenced by the Lean Startup Methodology by Eric Ries and
          Steve Blank.
        </li>
        <li>My cat's name is Zelda, but I have never played the game.</li>
        <li>
          I have a big interest in wine. My long-term goal is to become a
          sommelier, but for the short-term, I want to attend as many wine
          tasting events as possible.
        </li>
        <li>
          I'm a self-proclaimed psychologist, watching reality dating shows and
          giving relationship advice to people I've never met
        </li>
        <li>If it tells you anything, I'm an ESTJ, an Executive.</li>
      </ul>
    </div>
  </div>
</section>
