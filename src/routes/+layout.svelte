<script lang="ts">
    import Nav from '../components/navbar.svelte';
  </script>

<style>
  body {
     background-color: #000;
     color: #fff;
     font-family: 'Montserrat', sans-serif;
  }
 </style>
 <Nav />
 
   <div class="container">
     <slot></slot>
   </div>
   <body></body>
 
