<script>
    import { page } from '$app/stores';
    let links = [
        {
            title: "Home",
            path: "/",
        },
        {
            title: "About",
            path: "/about",
        },
        {
            title: "Contact",
            path: "/contact",
        },
        {
            title: "Pricing",
            path: "/pricing",
        },
        {
            title: "FAQ",
            path: "/faq",
        },
    ];
</script>

<nav class="navbar navbar-expand-md navbar-dark bg-dark" data-bs-theme="dark">
  <div class="container-fluid">
    <a class="navbar-brand fw-bold" href="/">SpyderByte</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <!-- Navbar menus -->
      <ul class="navbar-nav mx-auto mb-2 mb-lg-0">
        {#each links as link}
        <li class="nav-item">
          <a class="nav-link" class:active={link.path === $page.url.pathname} aria-current={link.path === $page.url.pathname} href="{link.path}">{link.title}</a>
        </li>
        {/each}
      </ul>
      <!-- Social media icons -->
      <ul class="navbar-nav sm-icons">
        <li>
          <a class="icon-link" href="https://facebook.com/">
            <svg class="bi" aria-hidden="true"><use xlink:href="#facebook"></use></svg>
          </a>
        </li>
        <li><a class="nav-link" href="/">hey<i class="bi bi-instagram"></i></a></li>
        <li><a class="nav-link" href="/">yo<i class="bi bi-twitter"></i></a></li>
        <li><a class="nav-link" href="/">dad<i class="bi bi-pinterest"></i></a></li>
      </ul>
    </div>
  </div>
</nav>
