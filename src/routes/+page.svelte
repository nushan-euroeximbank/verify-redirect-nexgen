<div class="container">
  <div class="loader"></div>
  <h1>Redirecting you</h1>
  <p>If you are not redirected automatically, <a href="https://nexgenrecruit.com/verify">click here</a></p>
</div>

<script>
  import { onMount } from "svelte";

  onMount(() => {
    setTimeout(() => {
      window.location.href = "https://nexgenrecruit.com/verify";
    }, 500);
  });
</script>

<style>
  .container {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #f5f7f3;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
  }

  h1 {
    color: #4a5844;
    font-size: 1.8rem;
    font-weight: 600;
    margin: 1.5rem 0 0.5rem 0;
  }

  p {
    color: #5f6b58;
    font-size: 1rem;
  }

  a {
    color: #7c8b73;
    text-decoration: none;
    transition: color 0.2s ease;
  }

  a:hover {
    color: #5f6b58;
    text-decoration: underline;
  }

  .loader {
    width: 48px;
    height: 48px;
    border: 5px solid #e2e8dc;
    border-bottom-color: #7c8b73;
    border-radius: 50%;
    animation: rotation 1s linear infinite;
  }

  @keyframes rotation {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }
</style>
