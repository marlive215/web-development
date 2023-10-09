<script lang="ts">
    import Nav from '../components/navbar.svelte';
    import Footer from '../components/footer.svelte';
  </script>

<style>
  body {
     background-color: black;
     color: #fff;
     font-family: 'Montserrat', sans-serif;
     padding-top: 110px; 
  }
 </style>
 <Nav />
 
   <div class="container-fluid">
     <slot></slot>
   </div>
   <body></body>

  <Footer />
 
