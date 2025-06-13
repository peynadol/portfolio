<script>
  import Separator from "./Separator.svelte";
</script>

<section class="my-16 text-left">
  <Separator />
  <h2 class="heading-m mb-4 underline underline-accent">
    Skills & Technologies
  </h2>

  <div class="grid gap-10 md:grid-cols-2">
    <div>
      <h3 class="font-bold text-lg mb-1">Core Frontend</h3>
      <ul class="list-disc list-inside text-base">
        <li>HTML, CSS, JavaScript, TypeScript</li>
        <li>React, Next.js, Tailwind CSS</li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Form Handling & Validation</h3>
      <ul class="list-disc list-inside text-base">
        <li>React Hook Form</li>
        <li>Zod</li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Backend & Full Stack</h3>
      <ul class="list-disc list-inside text-base">
        <li>Node.js, Express, PostgreSQL</li>
        <li>
          Comfortable building APIs, connecting to databases, and deploying
          full-stack apps
        </li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Testing & Tooling</h3>
      <ul class="list-disc list-inside text-base">
        <li>Git & GitHub for version control</li>
        <li>Deployments with Vercel and Render</li>
        <li>Basic experience with Vitest, Jest, and Playwright</li>
      </ul>
    </div>
  </div>
</section>
