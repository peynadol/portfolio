<script lang="ts">
  import { toast } from "svelte-5-french-toast";

  let name = "";
  let email = "";
  let message = "";
  let isSubmitting = false;

  async function handleSubmit(event: Event) {
    event.preventDefault();
    isSubmitting = true;

    const formData = new FormData();
    formData.append("name", name);
    formData.append("email", email);
    formData.append("message", message);

    try {
      const res = await fetch("https://formspree.io/f/xvgrjqdr", {
        method: "POST",
        body: formData,
        headers: {
          Accept: "application/json",
        },
      });

      if (res.ok) {
        toast.success("Message sent!");
        name = email = message = "";
      } else {
        toast.error("Something went wrong. Please try again.");
      }
    } catch (err) {
      toast.error("Network error. Try again later.");
    } finally {
      isSubmitting = false;
    }
  }
</script>

<section id="contact" class=" py-20 px-6 md:px-12 border-b border-white">
  <div class="max-w-2xl mx-auto text-left">
    <h2 class="heading-l text-white mb-6">Contact</h2>

    <p class="body-l text-muted mb-12">
      I would love to hear about your project and how I could help. Please fill
      in the form, and I’ll get back to you as soon as possible.
    </p>

    <form on:submit={handleSubmit} autocomplete="off" class="space-y-8">
      <input type="text" name="_gotcha" class="hidden" />

      <input
        type="text"
        name="name"
        placeholder="NAME"
        bind:value={name}
        required
        class="w-full bg-transparent border-b border-white py-3 text-white placeholder:text-muted focus:outline-none focus:ring-accent focus:border-accent"
      />

      <input
        type="email"
        name="email"
        placeholder="EMAIL"
        bind:value={email}
        required
        class="w-full bg-transparent border-b border-white py-3 text-white placeholder:text-muted focus:outline-none focus:ring-accent focus:border-accent"
      />

      <textarea
        name="message"
        rows="4"
        placeholder="MESSAGE"
        bind:value={message}
        required
        class="w-full bg-transparent border-b border-white py-3 text-white placeholder:text-muted focus:outline-none focus:ring-accent focus:border-accent"
      ></textarea>

      <button
        type="submit"
        class="uppercase font-bold tracking-widest text-white group cursor-pointer relative"
        disabled={isSubmitting}
      >
        {isSubmitting ? "Sending..." : "Send Message"}
        <span class="block h-[2px] w-full bg-accent mt-2"></span>
      </button>
    </form>
  </div>
</section>
