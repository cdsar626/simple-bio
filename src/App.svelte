<script lang="ts">
  import Card from './lib/Card.svelte';
</script>

<main>
  <div>
    <a href="https://www.linkedin.com/in/cdsar626/" target="_blank" rel="noreferrer">
      <img src="https://media.licdn.com/dms/image/C4D35AQEoJ7NB80W0eA/profile-framedphoto-shrink_400_400/0/1592957635473?e=1698973200&v=beta&t=tV99DRHLy0Omv5UjEAMJPfgXKR6qizc7v5vn9qPD3NM" class="logo" alt="LinkedIn_pfp" />
    </a>
  </div>
  <h1>Cesar De la Vega Salinas</h1>
  <h4>Software Developer / Fullstack</h4>

  <div class="projects">
    <Card title={"Basic Personal Server"}
    description={"A basic server to upload files, built in vuejs and expressjs."}
    url={"https://files.cdsar626.com"}
    />
    <Card title={"eCommerce Clone"}
    description={"A clone of Andreas Kitchen Meals website, using shoprocket store instead of Wix's. Built using Astro/Solidjs/TailwindCSS."}
    url={"https://akm.cdsar626.com"}
    />
    <Card class="span2" title={"Tablist"}
    description={"A Work-in-progress task list app. Now available only in Playstore. App built using flutter and mongodb."}
    url={"https://akm.cdsar626.com"}
    />
  </div>

  <p>
    Check out <a href="https://github.com/cdsar626" target="_blank" rel="noreferrer">My Github</a>, there you will find the source codes and more projects.
  </p>

  <p>
    Click on profile picture to go to my <a href="https://github.com/cdsar626" target="_blank" rel="noreferrer">LinkedIn</a>.
  </p>
  <p class="read-the-docs">
    This website is also a work-in-progress :)
  </p>
</main>

<style>
  .projects {
    display: grid;
    grid-template-columns: auto auto;
    gap: 20px;
  }
  .logo {
    height: 8em;
    will-change: filter;
    transition: filter 300ms;
    border: 1px;
    border-radius: 50%;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
