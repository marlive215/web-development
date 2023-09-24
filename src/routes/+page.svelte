<script>
	import { onDestroy } from "svelte";

  let words = ["BUSINESS", "VENTURE", "BRAND", "FIRM", "WEBSITE", "ORGANIZATION", "IDEA"];
  let currentWordIndex = 0;

  function changeWord() {
    currentWordIndex = (currentWordIndex + 1) % words.length;
  }

  // Set an interval to change the word every few seconds
  const interval = setInterval(changeWord, 700);

  // Clear the interval when the component is destroyed to prevent memory leaks
  onDestroy(() => {
    clearInterval(interval);
  });
</script>


<main>

    <style>
        main {
          display: flex;
          justify-content: center;
          align-items: center;
          height: 100vh; 
        }
        .hero {
          text-align: center;
          padding: 50px 0;
          background-color: #000; 
        }
      
        .title {
          font-family: 'Montserrat', sans-serif;
          font-size: 72px;
          font-weight: bold;
          margin-bottom: 10px;
          position: relative;
          /* display: flex; 
          align-items: baseline;  */
        }

        .changing-word {
          color: #FF1616;
          animation: slide-up 1s ease infinite alternate;
        }

        @keyframes slide-up {
          0% {
            transform: translateY(0);
          }
          100% {
            transform: translateY(-20px); /* Adjust the distance of the slide */
          }
         } 
      
        .subtitle {
          font-family: 'Montserrat', sans-serif;
          font-size: 72px;
          font-weight: bold;
          margin-bottom: 20px;
        }
      
        .mission {
          font-family: 'Montserrat', sans-serif;
          font-size: 22px;
          margin-bottom: 30px;
        }
      
        .learn-more-button {
        background-color: #FF1616;
        color: #fff;
        font-weight: bold;
        font-size: 16px;
        padding: 10px 20px;
        border: none;
        cursor: pointer;
        transition: background-color 0.3s;
        border-radius: 50px; /* Adjust the value to control the roundness */
    }
      
        .learn-more-button:hover {
          background-color: #fff;
          color: #FF1616;
    
        }
        .learn-more-button-link {
            color: #fff;
            text-decoration: none;
        }
      </style>


    <div class="hero">
      <div class="title">
        <span>ELEVATE YOUR </span><span class="changing-word">{words[currentWordIndex]}</span>
      </div>
      <div class="subtitle">AND RUN THE WEB</div>
      <div class="mission">
        SpyderByte is a versatile digital agency specializing in website design and digital marketing solutions, dedicated to helping businesses thrive in the ever-evolving online landscape.
      </div>
      <button class="learn-more-button"><a class="learn-more-button-link" href="/about">Learn more</a></button>
    </div>

</main>