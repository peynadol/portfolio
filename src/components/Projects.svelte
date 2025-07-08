<script>
  import ProjectCard from "./ProjectCard.svelte";
  import Separator from "./Separator.svelte";
</script>

<section class="my-16 text-left" id="projects">
  <Separator />
  <h2 class="heading-m mb-8">Projects</h2>

  <div class="space-y-10">
    <ProjectCard
      title="Personal Finance Dashboard"
      description="A personal finance tracker built with Next.js and Supabase. Features dynamic budgeting, savings goals (“pots”), and transaction history. Built to deepen my understanding of full-stack app structure, state management with TanStack Query, and TypeScript integration."
      tech={["Next.js", "Typescript", "TanStack Query", "Supabase"]}
      live="https://finance-h78h.vercel.app/"
      github="https://github.com/peynadol/finance"
      image="/images/finance-app-preview.png"
    />

    <ProjectCard
      title="Product Feedback App"
      description="A responsive web app for submitting and discussing product feedback. Features voting, filtering, nested comments, and a detailed suggestion board."
      tech={["Next.js", "TypeScript", "Tailwind", "Zustand"]}
      live="https://product-feedback-app-gray.vercel.app/"
      github="https://github.com/peynadol/product-feedback-app"
      image="/images/product-feedback-preview.jpeg"
    />
    <ProjectCard
      title="GitHub Issue Viewer"
      description="A lightweight web app to browse GitHub issues using the GitHub API. Implements data caching and pagination with React Query for a smooth experience."
      tech={["React", "TypeScript", "React Query", "Tailwind", "GitHub API"]}
      live="https://github-issue-viewer-ashy.vercel.app/"
      github="https://github.com/peynadol/github-issue-viewer"
      image="/images/github-issue-viewer-preview.png"
    />

    <ProjectCard
      title="Multi-Step Form"
      description="A polished multi-step form with validation using Zod and React Hook Form. Supports step navigation, error handling, and a toast notification on submission."
      tech={["React", "TypeScript", "React Hook Form", "Zod", "Tailwind"]}
      live="https://multi-step-form-tau-ashen.vercel.app/"
      github="https://github.com/peynadol/multi-step-form"
      image="/images/multi-step-form-preview.jpeg"
    />

    <ProjectCard
      title="Planetary Facts"
      description="A responsive, modern web app built with Next.js 15, React 19, and Tailwind CSS 4, showcasing facts and visuals about the planets in our solar system."
      tech={["Next.js", "JavaScript", "Tailwind"]}
      live="https://planet-facts-gamma.vercel.app/planets/mercury"
      github="https://github.com/peynadol/planet-facts"
      image="/images/planetary-facts-preview.jpeg"
    />

    <ProjectCard
      title="MyTeam Landing Page"
      description="A responsive marketing site built with Svelte and Tailwind CSS. Designed to showcase clean layout structure, mobile-first responsiveness, and component reuse."
      tech={["Svelte", "Tailwind", "TypeScript"]}
      live="https://myteam-dusky.vercel.app/"
      github="https://github.com/peynadol/myteam"
      image="/images/myteam-landing-page-preview.jpeg"
    />
  </div>
</section>
