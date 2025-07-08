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
      <ul class="list-disc list-outside pl-5 text-base">
        <li>Semantic HTML, modern CSS, JavaScript (ES6+)</li>
        <li>React & Next.js (app and pages routers)</li>
        <li>TypeScript (basic to intermediate use)</li>
        <li>Tailwind CSS</li>
        <li>RHF and Zod for form handling and validation</li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Backend & Full Stack</h3>
      <ul class="list-disc list-outside pl-5 text-base">
        <li>Node.js, Express, PostgreSQL (basic to intermediate)</li>
        <li>Experience building APIs and connecting to databases</li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Testing & Tooling</h3>
      <ul class="list-disc list-outside pl-5 text-base">
        <li>Version control with Git & GitHub</li>
        <li>Deployments with Vercel and Render</li>
        <li>Working knowledge of Vitest, Jest, and Playwright</li>
      </ul>
    </div>

    <div>
      <h3 class="font-bold text-lg mb-1">Exploring</h3>
      <ul class="list-disc list-outside pl-5 text-base">
        <li>PHP & Laravel</li>
        <li>Accessibility best practices</li>
        <li>TanStack (Query, Router, Table)</li>
        <li>Frontend performance optimization</li>
      </ul>
    </div>
  </div>
</section>
