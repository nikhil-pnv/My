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
      
      return () => clearInterval(interval); // Cleanup on component destroy
    });
  </script>
  <div class="typing-effect">{typing}</div>
  
  <style>
    
    .typing-effect {
    white-space: pre;
    overflow: hidden;
    animation: blinkingCursor 5s infinite;
    position: absolute;
    color: rgb(229, 73, 11);
    text-shadow: 1px 1px #252424;
    top: 90%;
    left: 25%;
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

/* For tablets and smaller devices */
@media (max-width: 768px) {
    .typing-effect {
        position: absolute;
        font-size: 2rem;
        top: 75%;   /* You can adjust these based on how it looks on tablet screens */
        left: 15%;
    }
}

/* For mobile devices */
@media (max-width: 480px) {
    .typing-effect {
        position: absolute;
        font-size: 0.8rem;
        top: 75%;   /* You can adjust these based on how it looks on mobile screens */
        left : 25%;
    }
}

  </style>
  
