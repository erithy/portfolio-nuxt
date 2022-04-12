<!-- Please remove this file from your project -->
<template>
  <div class="relative flex items-top justify-center container mx-auto md:px-12 min-h-screen items-center">
    <div class="text-center md:grid md:grid-cols-2 md:gap-2 z-10">
      <!-- <div class="loader">
      </div> -->
        <img
          src="https://mdbcdn.b-cdn.net/img/new/avatars/8.webp"
          class="rounded-full w-40 md:w-80 mx-auto"
          alt="Avatar"
        />
        <div class="flex flex-col justify-center px-2">
          <div class="ma-auto py-5">
            <span class="subheading text-base sm:text-3xl font-bold">Hello! I am</span>
            <h5 class="text-xl sm:text-3xl font-medium leading-tight mb-2">John Doe</h5>
            <p class="text-gray-400 sm:text-lg typing-text m-auto">I am a Web Developer.</p>
            <div class="flex justify-center pt-4 space-x-2">
              <a href="https://github.com/erithy" target="_blank"><svg
                class="w-6 h-6 dark:text-white dark:hover:text-blue-300 text-gray-600 hover:text-blue-300 button--github"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                width="32"
                height="32"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              ><path d="M12 2.247a10 10 0 0 0-3.162 19.487c.5.088.687-.212.687-.475c0-.237-.012-1.025-.012-1.862c-2.513.462-3.163-.613-3.363-1.175a3.636 3.636 0 0 0-1.025-1.413c-.35-.187-.85-.65-.013-.662a2.001 2.001 0 0 1 1.538 1.025a2.137 2.137 0 0 0 2.912.825a2.104 2.104 0 0 1 .638-1.338c-2.225-.25-4.55-1.112-4.55-4.937a3.892 3.892 0 0 1 1.025-2.688a3.594 3.594 0 0 1 .1-2.65s.837-.262 2.75 1.025a9.427 9.427 0 0 1 5 0c1.912-1.3 2.75-1.025 2.75-1.025a3.593 3.593 0 0 1 .1 2.65a3.869 3.869 0 0 1 1.025 2.688c0 3.837-2.338 4.687-4.563 4.937a2.368 2.368 0 0 1 .675 1.85c0 1.338-.012 2.413-.012 2.75c0 .263.187.575.687.475A10.005 10.005 0 0 0 12 2.247z" fill="currentColor" /></svg></a>
              <a href="https://twitter.com/nuxt_js" target="_blank"><svg
                class="w-6 h-6 dark:text-white dark:hover:text-blue-300 text-gray-600 hover:text-blue-300"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                aria-hidden="true"
                role="img"
                width="32"
                height="32"
                preserveAspectRatio="xMidYMid meet"
                viewBox="0 0 24 24"
              ><path d="M22.46 6c-.77.35-1.6.58-2.46.69c.88-.53 1.56-1.37 1.88-2.38c-.83.5-1.75.85-2.72 1.05C18.37 4.5 17.26 4 16 4c-2.35 0-4.27 1.92-4.27 4.29c0 .34.04.67.11.98C8.28 9.09 5.11 7.38 3 4.79c-.37.63-.58 1.37-.58 2.15c0 1.49.75 2.81 1.91 3.56c-.71 0-1.37-.2-1.95-.5v.03c0 2.08 1.48 3.82 3.44 4.21a4.22 4.22 0 0 1-1.93.07a4.28 4.28 0 0 0 4 2.98a8.521 8.521 0 0 1-5.33 1.84c-.34 0-.68-.02-1.02-.06C3.44 20.29 5.7 21 8.12 21C16 21 20.33 14.46 20.33 8.79c0-.19 0-.37-.01-.56c.84-.6 1.56-1.36 2.14-2.23z" fill="currentColor" /></svg></a>
            </div>
          </div>
        </div>
    </div>
    <!-- <div class="blob">
      <svg xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 310 350">
        <path d="M156.4,339.5c31.8-2.5,59.4-26.8,80.2-48.5c28.3-29.5,40.5-47,56.1-85.1c14-34.3,20.7-75.6,2.3-111  c-18.1-34.8-55.7-58-90.4-72.3c-11.7-4.8-24.1-8.8-36.8-11.5l-0.9-0.9l-0.6,0.6c-27.7-5.8-56.6-6-82.4,3c-38.8,13.6-64,48.8-66.8,90.3c-3,43.9,17.8,88.3,33.7,128.8c5.3,13.5,10.4,27.1,14.9,40.9C77.5,309.9,111,343,156.4,339.5z"/>
      </svg>
    </div> -->
  </div>
</template>

<script>
export default {
  name: 'NuxtTutorial'
}
</script>

<style>
.subheading {
    text-transform: uppercase;
    color: #90acd1;
    letter-spacing: 4px;
}
  /* * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #000;
  } */

  .loader {
    position: relative;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: linear-gradient(45deg, transparent, transparent 40%, #e5f403);
    animation: animate 2s linear infinite;
  }

  .loader:before {
    content: "";
    position: absolute;
    top: 6px;
    left: 6px;
    right: 6px;
    bottom: 6px;
    border-radius: 50%;
    z-index: 1000;
  }

  @keyframes animate {
    0% {
      transform: rotate(0deg);
      filter: hue-rotate(0deg);
    }

    100% {
      transform: rotate(360deg);
      filter: hue-rotate(360deg);
    }
  }

  .loader:after {
    content: "";
    position: absolute;
    top: 0px;
    left: 0px;
    right: 0px;
    botom: 0px;
    background: #000;
    background: linar-gradient(45deg, transparent, transparent 40%, #ffc300);
    border-radius: 50%;
    z-index: 1000;
    z-index: blur(10px);
  }
  .typing-text {
    width: 20ch;
    animation: typing 2s steps(20), blink .5s step-end infinite alternate;
    white-space: nowrap;
    overflow: hidden;
    border-right: 1px solid;
  }

  @keyframes typing {
    from {
      width: 0
    }
  }

  @keyframes blink {
    50% {
      border-color: transparent
    }
  }
  .blob {
    position: absolute;
    top: 0;
    left: 0;
    fill: #8bacdb33;
    width: 50vmax;
    z-index: 0;
    animation: move 15s ease-in-out infinite;
    transform-origin: 50% 50%;
  }

  @keyframes move {
    0%   { transform: scale(1)   translate(10px, -30px); }
    38%  { transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg); }
    40%  { transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg); }
    78%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg); }
    80%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg); }
    100% { transform: scale(1)   translate(10px, -30px); }
  }
</style>
