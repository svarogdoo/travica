<script>
  let name = "";
  let email = "";
  let subject = "";
  let message = "";

  $: isDisabled = !(name && email && subject && message);
</script>

<svelte:head>
  <title>Work with us</title>
  <meta name="description" content="Contact form for getting in touch" />
</svelte:head>

<section class="contact-section">
  <div class="contact-text">
    <h1 class="mt-56 lg:mt-20">HELLO THERE.</h1>
    <br />
    <p>
      If you require any information about our services, please get in touch.
    </p>

    <form
      class="w-full flex flex-col gap-y-4 mt-8"
      target="_blank"
      action="https://formsubmit.co/utravica@gmail.com"
      method="POST"
      id="contact"
    >
      <input
        type="text"
        name="name"
        id="name"
        class="px-8 py-4 w-full rounded-sm border bg-transparent border-fidelis-black placeholder:text-slate-200 placeholder:text-sm lg:placeholder:text-lg"
        placeholder="Name"
        bind:value={name}
      />
      <input
        type="email"
        name="email"
        id="email"
        class="px-8 py-4 w-full rounded-sm border bg-transparent border-fidelis-black placeholder:text-slate-200 placeholder:text-sm lg:placeholder:text-lg"
        placeholder="Email"
        bind:value={email}
      />
      <input
        type="text"
        name="subject"
        id="subject"
        class="px-8 py-4 w-full rounded-sm border bg-transparent border-fidelis-black placeholder:text-slate-200 placeholder:text-sm lg:placeholder:text-lg"
        placeholder="Subject"
        bind:value={subject}
      />
      <textarea
        name="message"
        id="message"
        class="px-8 py-4 w-full rounded-sm border bg-transparent border-fidelis-black placeholder:text-slate-200 placeholder:text-sm lg:placeholder:text-lg"
        placeholder="Message"
        bind:value={message}
        rows="7"
      />

      <input
        type="submit"
        class="bg-white text-black py-4 tracking-wider disabled:bg-gray-400 {!isDisabled
          ? 'cursor-pointer hover:scale-105 transition ease-in-out active:scale-95'
          : ''} "
        value="Send"
        disabled={isDisabled}
      />
    </form>

    <br />
    <br />
    <div class="flex flex-wrap gap-y-6 gap-x-6 justify-center">
      <a href="mailto:tcreativelab.contact@gmail.com"
        >tcreativelab.contact@gmail.com</a
      >
      <a target="_blank" href="https://www.instagram.com/TCREATIVELAB/"
        >@tcreativelab</a
      >
      <p>Youtube</p>
      <p>Linkedin</p>
    </div>

    <br />
    <br />
    <br />
  </div>
</section>

<style>
  section {
    color: whitesmoke;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-bottom: 10em;
    align-items: center;
    z-index: 10;
  }

  .contact-text {
    width: 30%;
    z-index: 10;
    margin-top: 7em;
  }
  h1 {
    font-size: 1.8em;
    letter-spacing: 0.1em;
    text-align: left;
  }

  p,
  a {
    font-size: 1.1em;
    letter-spacing: 0.05em;
    font-weight: 50;
    word-spacing: 0.15em;
    text-align: justify;
  }
  @media (max-width: 768px) {
    .contact-text {
      width: 85%;
      margin-top: 5em;
    }

    h1 {
      font-size: 1.1em;
    }

    p,
    a {
      font-size: 0.9em;
      letter-spacing: 0.05em;
      font-weight: 50;
      word-spacing: 0.1em;
      text-align: justify;
    }
  }
</style>
