<script>
  import { onDestroy } from "svelte";

  let words = ["BUSINESS", "VENTURE", "BRAND", "FIRM", "WEBSITE", "ORGANIZATION", "IDEA"];
  let currentWordIndex = 0;

  function changeWord() {
    currentWordIndex = (currentWordIndex + 1) % words.length;
  }

  // Set an interval to change the word every few seconds
  const interval = setInterval(changeWord, 500);

  // Clear the interval when the component is destroyed to prevent memory leaks
  onDestroy(() => {
    clearInterval(interval);
  });
</script>

<main class="min-vh-100 d-flex flex-column"> 
  <section class="hero-section bg-dark text-light position-relative">
 
    <div class="ratio ratio-16x9">
      <video autoplay muted loop id="background-video" style="object-fit-scale">
        <source src="src/videos/pexels-artem-podrez-5725960 (2160p).mp4" type="video/mp4">
      </video>
    </div>
    <div class="container d-flex justify-content-center align-items-center" style="position: relative; z-index: 2;">
      <div class="text-center p-5">
        <h1 class="title display-2 font-weight-bold mb-4">
          <span>ELEVATE YOUR BRAND</span>
        </h1>
        <h2 class="subtitle display-4 font-weight-bold mb-5">AND RUN THE WEB</h2>
        <a href="/about" class="btn btn-danger btn-lg">
          Learn more
        </a>
      </div>
    </div>
  </section>

  <section class="about-section bg-white py-3"> 
    <div class="container-fluid text-center text-dark min-vh-100">
      <h3 class="section-title display-4 font-weight-bold mb-4">About Us</h3>
      <p class="section-content lead mb-5">
        We are a passionate team of digital experts dedicated to helping businesses succeed online. With years of experience in website design, digital marketing, and branding, we have the skills and creativity to take your online presence to the next level.
      </p>
      <a href="/about" class="btn btn-primary btn-lg">
        Learn More
      </a>
    </div>
  </section>

  <section class="middle-section bg-white py-3"> 
    <div class="container-fluid text-center text-dark min-vh-100"> 
      <h3 class="section-title display-4 font-weight-bold mb-4">Our Services</h3>
      <p class="section-content lead mb-5">
        We offer a wide range of digital services to help you succeed online. Whether you need a stunning website, effective digital marketing strategies, or creative branding solutions, we've got you covered.
      </p>
      <a href="/services" class="btn btn-primary btn-lg">
        Explore Services
      </a>
    </div>
  </section>

  <section class="bottom-section bg-white py-3">
    <div class="container-fluid text-center text-dark min-vh-100"> 
      <h3 class="section-title display-4 font-weight-bold mb-4">Contact Us</h3>
      <p class="section-content lead mb-5">
        Ready to take your business to the next level? Contact us today to discuss your project and discover how we can help you achieve your online goals.
      </p>
      <a href="/contact" class="btn btn-success btn-lg">
        Get in Touch
      </a>
    </div>
  </section>
</main>
