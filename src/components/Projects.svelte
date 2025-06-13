<script>
  import ProjectCard from "./ProjectCard.svelte";
</script>

<section class="my-16 text-left" id="projects">
  <h2 class="heading-m mb-8">Projects</h2>

  <div class="space-y-10">
    <ProjectCard
      title="HMCTS Caseworker Task App"
      description="A task manager application for a developer challenge. Built with React, includes task flow, filters, and UI state."
      tech={["React", "JavaScript", "Tailwind"]}
      live="https://hmcts-caseworker-task-app.onrender.com/"
      github="https://github.com/peynadol/hmcts-caseworker-task-app"
    />
    <ProjectCard
      title="Planetary Facts"
      description="A responsive, modern web app built with Next.js 15, React 19, and Tailwind CSS 4, showcasing facts and visuals about the planets in our solar system."
      tech={["Next.js", "JavaScript", "Tailwind"]}
      live="https://planet-facts-gamma.vercel.app/planets/mercury"
      github="https://github.com/peynadol/planet-facts"
    />
    <ProjectCard
      title="Multi-Step Form"
      description="A multi-step form built with React Hook Form and Zod for validation. Features include dynamic step navigation, form state management, and responsive design."
      tech={["React", "TypeScript", "React Hook Form", "Zod"]}
      live="https://multi-step-form-5tct-1f8m7b2pd-liams-projects-d672842b.vercel.app/"
      github="https://github.com/peynadol/multi-step-form/tree/main"
    />
  </div>
</section>
