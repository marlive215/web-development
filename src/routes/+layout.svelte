<script lang="ts">
    import Nav from '../components/navbar.svelte';
  </script>


<style>
 body {
    background-color: #000;
    color: #fff;
    font-family: 'Montserrat', sans-serif;
 }

 .container {
    display: flex;
    flex-direction: column;
    align-items: center; /* Center vertically */
    width: 100%;
    max-width: 1200px; /* Adjust this to your desired max width */
}

</style>
<Nav />

  <div class="container">

    <slot></slot>
  </div>
  <body>

  </body>