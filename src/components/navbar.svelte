<script>
    import { page } from '$app/stores';
 
  
    let links = [
      {
        title: "About",
        path: "/about",
      },
      {
        title: "Products",
        path: "/products",
      },
    ];
  

  </script>
  
  <!DOCTYPE html>
  <html lang="eng">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.5.0/dist/css/bootstrap.min.css">
  </head>
  <body>
    <nav class="navbar fixed-top navbar-expand-lg navbar-dark bg-black py-4">
      <div class="container-fluid">
        <a class="navbar-brand" href="/">
            <img id="spyder-logo" src="src/imgs/mainlogo.png" alt="Logo" class="logo-img" style="max-width: 25em;">
        </a>
        <div class="collapse navbar-collapse">
        <ul class="navbar-nav ml-auto">
          {#each links as link}
          <li class="nav-item">
              <a class="nav-link {link.path === $page.url.pathname ? 'active fw-normal fs-5' : 'text-white fw-normal fs-5' } px-4" href="{link.path}" style="{link.path === $page.url.pathname ? 'color: #CCCCCC;': ''}">
                  {link.title}
                </a>
          </li>
          {/each}
        </ul>
        </div>
        <div class="d-grid gap-2 col-2 mx-auto">
          <a class="btn btn-lg btn-outline-danger ms-3 rounded-0 mx-3" href="/contact">Contact Us</a>
        </div>
      </div>
    </nav>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.5.0/dist/js/bootstrap.min.js"></script>
  </body>
  </html>
  
