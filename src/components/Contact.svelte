<section
  id="contact"
  class="bg-[#1A1A1A] py-20 px-6 md:px-12 border-b border-white"
>
  <div class="max-w-2xl mx-auto text-left">
    <h2 class="heading-l text-white mb-6">Contact</h2>

    <p class="body-l text-muted mb-12">
      I would love to hear about your project and how I could help. Please fill
      in the form, and I’ll get back to you as soon as possible.
    </p>

    <form
      action="https://formspree.io/f/xvgrjqdr"
      method="POST"
      autocomplete="off"
      class="space-y-8"
    >
      <input type="text" name="_gotcha" style="display: none;" />

      <input
        type="text"
        name="name"
        placeholder="NAME"
        required
        class="w-full bg-transparent border-white py-3 text-white placeholder:text-muted"
      />

      <input
        type="email"
        name="email"
        placeholder="EMAIL"
        required
        class="w-full bg-transparent border-white py-3 text-white placeholder:text-muted"
      />

      <textarea
        name="message"
        rows="4"
        placeholder="MESSAGE"
        required
        class="w-full bg-transparent border-white py-3 text-white placeholder:text-muted"
      ></textarea>

      <button
        type="submit"
        class="uppercase font-bold tracking-widest text-white group underline underline-accent cursor-pointer"
      >
        Send Message
        <span class="block h-[2px] w-full bg-accent mt-2"></span>
      </button>
    </form>
  </div>
</section>
