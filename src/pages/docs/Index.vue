<template>
  <Layout>
    <section class="container mx-auto">
      <div class="subheader">
        <h1>Get started in seconds</h1>
        <p>Step-by-Step Guide</p>
      </div>
      <div class="content">
        <h2>Getting started with BuildWith IONOS</h2>
        <p>
          In this tutorial, we will show you how easy it is to launch your site
          with BuildWith IONOS.
        </p>
        <h2>Step 1: Start</h2>
        <p>
          <a
            class="self-center md:self-start pb-8 md:pb-0"
            href="https://buildwith.ionos.com/setup?repo=https://github.com/buildwith-ionos/buildwith-ionos-starter"
            rel="noopener"
            target="_blank"
          >
            <button
              class="text-white font-bold rounded-full bg-blue-600 inline-flex items-center shadow-lg focus:outline-none px-8 my-6 py-4"
            >
              <span>Drop to IONOS.space</span>
            </button>
          </a>
          is probably the easiest way to start.
        </p>
        <p>
          Or you <a href="https://buildwith.ionos.com/">login</a> the classic
          way. The only thing you need is an existing IONOS contract. If you
          have not already an IONOS contract, go ahead and
          <a href="https://www.ionos.com/">sign up</a> for a new one.
        </p>
        <p />
        <picture class="w-full">
          <source srcset="@images/get-started-01.webp" type="image/webp" />
          <source srcset="@images/get-started-01.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-01.webp"
            fit="contain"
            alt="Screenshot of BuildWith IONOS login"
          />
        </picture>
        <h2>Step 2: Connect to GitHub</h2>
        <p>BuildWith IONOS requisites your GitHub account:</p>
        <picture class="w-full">
          <source srcset="@images/get-started-02.webp" teype="image/webp" />
          <source srcset="@images/get-started-02.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-02.webp"
            fit="contain"
            alt="Screenshot of GitHub connect"
          />
        </picture>
        <p>
          Click the <b>Connect to GitHub</b> button as illustrated in the
          screenshot above.
        </p>
        <h2>Step 3: Authorize BuildWith IONOS</h2>
        <picture class="w-full">
          <source srcset="@images/get-started-03.webp" teype="image/webp" />
          <source srcset="@images/get-started-03.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-03.webp"
            fit="contain"
            alt="Screenshot of authorization"
          />
        </picture>
        <p>
          It's time to allow BuildWith IONOS and GitHub to talk to each other.
          Clicking the Authorize Application button will do just that. Like it
          says in the image above, BuildWith IONOS doesn't store your GitHub
          access token on our servers.
        </p>

        <h2>Step 4: Configure your project</h2>
        <picture class="w-full">
          <source srcset="@images/get-started-04.webp" teype="image/webp" />
          <source srcset="@images/get-started-04.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-04.webp"
            fit="contain"
            alt="Screenshot of project configuration"
          />
        </picture>
        <p>
          If you followed <i>Drop to IONOS.space</i> the source is automatically
          given. But you're free to choose your own project. Or simply use one
          of our starters to get familiar with BuildWith IONOS and create your
          first live web project in seconds. Click on <b>Continue</b> to
          initialize, build &amp; drop your first web project to IONOS.space.
        </p>
        <h2>
          Step 5: Initialize, Build &amp; Drop your first project to IONOS
        </h2>
        <picture class="w-full">
          <source srcset="@images/get-started-05-1.webp" teype="image/webp" />
          <source srcset="@images/get-started-05-1.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-05-1.webp"
            fit="contain"
            alt="Screenshot of project initialization"
          />
        </picture>
        <p>
          Now, we are starting to setup everything properly for you. Depending
          on the project size this step lasts for longer.
        </p>
        <picture class="w-full">
          <source srcset="@images/get-started-05-2.webp" teype="image/webp" />
          <source srcset="@images/get-started-05-2.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-05-2.webp"
            fit="contain"
            alt="Screenshot of project congrats"
          />
        </picture>
        <p>
          Hopefully, everything goes well all the time, you will see a success
          message. Click on <b>View project details</b> to get a detail summary
          of your project.
        </p>
        <picture class="w-full">
          <source srcset="@images/get-started-05-3.webp" teype="image/webp" />
          <source srcset="@images/get-started-05-3.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-05-3.webp"
            fit="contain"
            alt="Screenshot of project details"
          />
        </picture>
        <p>
          Now, your workflow with
          <a href="https://github.com/features/actions">GitHub Actions</a>
          should run automatically. You can check on GitHub directly or stay
          tuned on our detail page. Progress is indicated by <b>state</b> and a
          thumbnail screenshot as soon as your project is successful dropped to
          IONOS.
        </p>
        <h2>Step 6: All done</h2>
        <p>
          Once the build completes, your site is live! Head to the generated URL
          of your newly published site:
        </p>
        <picture class="w-full">
          <source srcset="@images/get-started-06.webp" teype="image/webp" />
          <source srcset="@images/get-started-06.webp.png" type="image/png" />
          <g-image
            src="@images/get-started-06.webp"
            fit="contain"
            alt="Screenshot of resulting web project"
          />
        </picture>
        <p>
          Now, you should have a copy of this website on your own. Congrats, and
          thanks for using BuildWith IONOS!
        </p>
      </div>
    </section>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Get started',
  },
}
</script>
