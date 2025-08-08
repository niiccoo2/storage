<svelte:head>
    <title>Storage - YSWS</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400..700&family=Google+Sans+Code:ital,wght@0,300..800;1,300..800&family=Londrina+Shadow&family=Nata+Sans:wght@100..900&family=Orbitron:wght@400..900&display=swap" rel="stylesheet">
</svelte:head>


<style>
    .title_wrapper {
    position: relative;
    width: 100%;
    height: auto;
    }

    .title_top {
        position: static; 
        display: block;
        margin: 0 auto;
        max-width: 100%;
        padding: 0.5em;
    }

    .explanation_wrapper {
        position: relative;
        width: 100%;
        min-height: 150px;
        margin-top: 1em;
    }


    .explanation_text {
        position: static;
        font-size: clamp(1.5rem, 5vw, 2rem);
        text-shadow: 1px 1px 3px #a0e0f4;
        text-align: center;
        color: #3853a1;
        user-select: none;
        margin: 0.1rem;
        transition: color 0.3s ease, transform 1s ease-in-out;

        padding: 0.5em 3em;
        
    }

    .google-sans-code {
  font-family: "Google Sans Code", monospace;
  font-optical-sizing: auto;
  font-weight: 2px;
  font-style: normal;
}


@keyframes wiggle {
  0%, 100% { transform: translate(0, 0) rotate(0deg); }
  25% { transform: translate(-2px, 0.5px) rotate(-1deg); }
  50% { transform: translate(2px, 0.5px) rotate(1deg); }
  75% { transform: translate(-2px, 0) rotate(-0.5deg); }
}

.wiggle {
    animation: wiggle 3s ease-in-out infinite;
    animation-iteration-count: 1;
    animation-delay: 2s;
    animation-fill-mode: forwards;
}

@keyframes wobble {
  0%, 100% { transform: translate(0, 0) rotate(0deg); }
  25% { transform: translate(0px, 0px) rotate(-0.5deg); }
  75% { transform: translate(0px, 0) rotate(0.5deg); }
}

.wobble {
    animation: wobble 2s ease-in-out infinite;
}
.explanation_text:hover {
  animation: wiggle 0.5s ease-in-out 1 forwards;
  animation-play-state: running;

  color: #60a0f8;
  transform-origin: center;
  
}

</style>

<body style="overflow: hidden;">
    <div class="title_wrapper"> <!-- Title Img -->
        <img src="images/Storage_Title_And_Logo.png" alt="Storage Title And Logo" class="title_top wiggle">

        <div class="explanation_wrapper google-sans-code">
            <p class="explanation_text">You ship a script related to storage, we ship you computer storage!</p>
        </div>
    </div>
</body>