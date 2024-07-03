<script>
  import { page } from '$app/stores';
</script>

<style>
  .floating-actions {
    position: fixed;
    z-index: 14;
    background-color: var(--dark);
    bottom: 16px;
    border-radius: 32px;

    box-shadow:
      0 1px 18px 0 rgb(0 0 0 / 12%),
      0 6px 10px 0 rgb(0 0 0 / 14%),
      0 3px 5px -1px rgb(0 0 0 / 20%);
    left: 50%;
    transform: translateX(-50%);
    max-height: 70px;
  }

  ul {
    display: flex;
    flex-wrap: nowrap;
    list-style-type: none;
    padding: 0 6px;
  }

  li {
    text-decoration: none;
    white-space: nowrap;
    padding: 3px;
  }

  a {
    color: var(--pure-white);
    text-decoration: none;
    padding: 12px;
    border-radius: 12px;
    font-size: 12px;
  }

  a:hover {
    background-color: var(--text-color);
    color: var(--pure-white);
    text-decoration: none;
    border-radius: 24px;
  }

  @media (max-width: 720px) {
    .floating-actions {
      bottom: 8px;
    }

    a {
      color: var(--pure-white);
      padding: 8px;
      border-radius: 12px;
      font-size: 12px;
      line-height: 1px;
    }
    ul {
      padding: 6px 6px;
      margin: 10px;
    }

    li {
      padding: 0px;
    }
  }
</style>

<div class="floating-actions">
  <ul>
    <li class:active="{$page.url.pathname === '/'}">
      <a data-sveltekit-prefetch href="/">Home</a>
    </li>
    <li class:active="{$page.url.pathname === '/about'}">
      <a data-sveltekit-prefetch href="/about">About</a>
    </li>
    <li class:active="{$page.url.pathname === '/about'}">
      <a href="#top">👆</a>
    </li>
  </ul>
</div>
