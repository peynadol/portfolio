<script>
  import { Github, Linkedin } from "@lucide/svelte";
</script>

<footer class=" border-t border-white py-10 px-6 md:px-12 text-white">
  <div
    class="max-w-4xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6"
  >
    <h2 class="heading-m">liampeynado</h2>

    <div class="flex gap-6">
      <a
        href="https://github.com/peynadol"
        target="_blank"
        rel="noopener noreferrer"
        class="hover:text-accent transition-colors"
        aria-label="GitHub"
      >
        <Github />
      </a>

      <a
        href="https://www.linkedin.com/in/liam-peynado-7947b435a/"
        target="_blank"
        rel="noopener noreferrer"
        class="hover:text-accent transition-colors"
        aria-label="LinkedIn"
      >
        <Linkedin />
      </a>
    </div>
  </div>
</footer>
