<script>
    import { onMount } from 'svelte';
    let text = "Hey ! I'm  \n NIKHIL VARMA PINNAMARAJU \n I'm a \n Full Stack Developer \n& \nTester";
    let typing = "";
    let delay = 150;
  
    onMount(() => {
      let i = 0;
      const interval = setInterval(() => {
        typing += text.charAt(i);
        i++;
  
        if (i > text.length) {
          clearInterval(interval);
        }
      }, delay);
      
      return () => clearInterval(interval); 
    });
  </script>
  <div class="typing-effect">{typing}</div>
  
  <style>
    
    .typing-effect {
    white-space: pre;
    overflow: hidden;
    animation: blinkingCursor 5s infinite;
    position: absolute;
    color: rgb(63, 63, 242);
    text-shadow: 1px 1px #252424;
    top: 40vh;
    left: 25vh;
    font-weight: 900;
    font-size: 2rem;
    text-align: center;
    justify-content: center;
    scroll-behavior: auto;
}

@keyframes blinkingCursor {
    0% { opacity: 1; }
    50% { opacity: 0; }
    100% { opacity: 1; }
}

@media (max-width: 768px) {
    .typing-effect {
        position: absolute;
        font-size: 1rem;
        left: 10%;
        margin-top: 1%;
        margin-right: 0%;
    }
}
@media (max-width: 480px) {
    .typing-effect {
        position: absolute;
        font-size: 0.8rem;
        top: 35%; 
        left : 17%;
    }
}

  </style>
  
