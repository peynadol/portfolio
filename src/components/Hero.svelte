<script>
  import { onMount } from "svelte";

  let waving = true;

  onMount(() => {
    const timeout = setTimeout(() => {
      waving = false;
    }, 1800);

    return () => clearTimeout(timeout);
  });

  function reWave() {
    if (!waving) {
      waving = true;
      setTimeout(() => {
        waving = false;
      }, 1800);
    }
  }
</script>

<!-- TODO: add a contact me link which navigates to the contact section -->

<section class="my-4 mt-16">
  <h1 class="heading-l mb-4">
    Hi there
    <span
      class:wave={waving}
      on:mouseenter={reWave}
      aria-label="waving hand"
      role="img"
    >
      👋
    </span>, I'm <span class="underline underline-accent">Liam</span>.
  </h1>
  <p class="body-l">
    Self-taught, UK based, 3 years of learning and building. Looking for my
    first development role while exploring full-stack.
    <br />
    <button
      class=" mt-2 text-accent hover:underline hover:underline-accent hover:cursor-pointer transition-all duration-200"
    >
      More about me ↓
    </button>
  </p>
</section>

<style>
  @keyframes wave-animation {
    0% {
      transform: rotate(0deg);
    }
    10% {
      transform: rotate(14deg);
    }
    20% {
      transform: rotate(-8deg);
    }
    30% {
      transform: rotate(14deg);
    }
    40% {
      transform: rotate(-4deg);
    }
    50% {
      transform: rotate(10deg);
    }
    60% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(0deg);
    }
  }

  .wave {
    display: inline-block;
    transform-origin: 70% 70%;
    animation: wave-animation 1.8s ease-in-out;
  }
</style>
