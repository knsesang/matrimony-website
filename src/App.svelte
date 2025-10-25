<script>
  import Header from './components/Header.svelte'
  import Hero from './components/Hero.svelte'
  import Features from './components/Features.svelte'
  import Architecture from './components/Architecture.svelte'
  import Technology from './components/Technology.svelte'
  import Roadmap from './components/Roadmap.svelte'
  import Contact from './components/Contact.svelte'
  import Footer from './components/Footer.svelte'
</script>

<style global>
  :global(*) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  :global(body) {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    color: #333;
    background-color: #fff;
  }

  :global(a) {
    color: #e91e63;
    text-decoration: none;
  }

  :global(a:hover) {
    text-decoration: underline;
  }
</style>

<Header />
<Hero />
<Features />
<Architecture />
<Technology />
<Roadmap />
<Contact />
<Footer />

