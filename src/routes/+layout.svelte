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
     align-items: center; 
     width: 100%;
     max-width: 1200px; 
 }
 </style>
 <Nav />
 
   <div class="container">
     <slot></slot>
   </div>
   <body></body>
 