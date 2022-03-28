<script>
  import Button from "./Button.svelte";
  import Particles from "svelte-particles";

  let particlesConfig = {
    fpsLimit: 60,
    particles: {
      color: {
        value: "#000"
      },
      links: {
        enable: true,
        color: "#000"
      },
      move: {
        enable: true
      }
    }
  };
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
  }

  :global(#tsparticles) {
    margin: 0;
    padding: 0;
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    z-index: -1;
  }
</style>

<main>
	<h1>Hello CodeSandbox</h1>
	<h2>Start editing to see some magic happen!</h2>
	<Button />
  <Particles options={particlesConfig} />
</main>