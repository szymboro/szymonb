<template>
  <div class="h-screen sticky top-0">
    <div class="container mx-auto py-80">
      <Particles
        id="tsparticles"
        :particlesInit="particlesInit"
        :particlesLoaded="particlesLoaded"
        :options="{
          background: {
            color: {
              value: '#000',
            },
          },
          fpsLimit: 144,
          fullScreen: {
            enable: true,
            zIndex: -1,
          },

          interactivity: {
            detectsOn: 'window',
            events: {
              onClick: {
                enable: true,
                mode: 'push',
              },
              onHover: {
                enable: true,
                mode: 'grab',
              },
              resize: true,
            },
            modes: {
              bubble: {
                distance: 300,
                duration: 2,
                opacity: 0.8,
                size: 40,
              },
              push: {
                quantity: 4,
              },
              grab: {
                distance: 150,
                duration: 1,
              },
            },
          },
          particles: {
            color: {
              value: '#D100D1',
            },
            links: {
              color: '#D100D1',
              distance: 180,
              enable: true,
              opacity: 1,
              width: 1,
            },
            collisions: {
              enable: false,
            },
            move: {
              direction: 'none',
              enable: true,
              outMode: 'out',
              random: false,
              speed: 3,
              straight: false,
            },
            number: {
              density: {
                enable: true,
                value_area: 1000,
              },
              value: 60,
            },
            opacity: {
              value: 0.5,
            },
            shape: {
              type: 'circle',
            },
            size: {
              random: true,
              value: 3,
            },
          },
          detectRetina: true,
        }"
      />
      <p class="font-sans font-light h-20 text-white text-sm tracking-long">
        SZYMONB_ DEV
      </p>
      <p class="font-sans text-6xl h-28 text-white font-semibold">szymonb_</p>
      <p class="font-mono text-lg text-gray-400">Young dev with big dreams</p>
      <div class="w-0 pt-8 grid gap-16 grid-cols-4 text-white text-3xl">
        <a
          class="
            transition
            duration-300
            ease-in-out
            transform
            hover:-translate-y-1 hover:scale-110
          "
          href="https://github.com/szymboro"
          target="_blank"
          ><span
            class="iconify"
            data-icon="akar-icons:github-outline-fill"
          ></span>
        </a>
        <a
          class="
            transition
            duration-300
            ease-in-out
            transform
            hover:-translate-y-1 hover:scale-110
          "
          href="https://www.instagram.com/x0simon/"
          target="_blank"
          ><span class="iconify" data-icon="akar-icons:instagram-fill"></span>
        </a>
        <a
          class="
            transition
            duration-300
            ease-in-out
            transform
            hover:-translate-y-1 hover:scale-110
          "
          href="https://www.facebook.com/piekielniedlugikurak"
          target="_blank"
          ><span class="iconify" data-icon="bx:bxl-facebook"></span>
        </a>
        <a
          class="
            transition
            duration-300
            ease-in-out
            transform
            hover:-translate-y-1 hover:scale-110
          "
          href="https://www.twitch.tv/xosimon_"
          target="_blank"
          ><span class="iconify" data-icon="akar-icons:twitch-fill"></span>
        </a>
      </div>
    </div>
  </div>
  <div class="h-screen bg-black sticky top-0">
    <div class="container mx-auto py-60 pl-64">
      <div class="content flex w-3/4">
        <div class="py-3">
          <p class="font-mono text-6xl text-white">A FEW W0RDS AB0UT ME!</p>
          <p class="font-mono text-gray-300 text-base pt-8 w-5/6">
            I am web developer for 4 years now, I started by creating projects
            in Wordpress Cms and now I'm using Vue.js and React. You can find
            more information about me in my
            <a
              href="https://www.linkedin.com/in/szymon-borowiecki-b588b71a6/"
              target="_blank"
              style="text-decoration: underline; color: #d100d1"
              >Linkedin</a
            >
            or
            <a
              href="https://github.com/szymboro"
              target="_blank"
              style="text-decoration: underline; color: #d100d1"
              >GitHub</a
            >
          </p>
        </div>
        <div class="w-full"><img src="../src/assets/pfp.jpg" /></div>
      </div>
    </div>
  </div>
  <div class="h-screen bg-white sticky top-0">
    <div class="container mx-auto py-60 pl-50">
      <p class="font-mono text-6xl text-black">RECENET WEB PR0JECTS</p>
      <br />
      <div
        class="carousel"
        data-flickity='{ "pauseAutoPlayOnHover": false
,"imagesLoaded": true, "percentPosition": false , "autoPlay": true, "wrapAround": true
}'
      >
        <img src="../src/assets/projects/praca1.png" />

        <img src="../src/assets/projects/praca2.png" />

        <img src="../src/assets/projects/praca3.png" />

        <img src="../src/assets/projects/praca4.png" />

        <img src="../src/assets/projects/praca5.png" />

        <img src="../src/assets/projects/praca6.png" />

        <img src="../src/assets/projects/praca7.png" />
      </div>
    </div>
    <div class="grid grid-cols-3 pt-6"></div>
  </div>
  <div class="h-screen bg-black sticky top-0">
    <div class="container mx-auto py-60 pl-50">
      <p class="font-mono text-6xl text-white">RECENET PR0GRAMING PR0JECTS</p>
      <br />
      <div
        class="carousel"
        data-flickity="{ prevNextButtons: false,
pageDots: false }"
        style="
          * {
            box-sizing: border-box;
          }

          body {
            font-family: sans-serif;
          }

          .carousel-cell {
            width: 66%;
            height: 200px;
            margin-right: 10px;
            border-radius: 5px;
            counter-increment: carousel-cell;
          }
          .carousel-cell:before {
            display: block;
            text-align: left;
            content: counter(carousel-cell);
            line-height: 200px;
            font-size: 80px;
            color: white;
          }
        "
      >
        <div class="grid grid-cols-2 pt-6">
          <a
            class="text-6xl text-white"
            href="https://github.com/szymboro/vuenews"
            target="_blank"
            ><span class="iconify" data-icon="bx:bx-code-alt"></span> VueNews</a
          >
        </div>
      </div>
    </div>
    <div class="grid grid-cols-3 pt-6"></div>
  </div>
  <div class="h-screen bg-white sticky top-0">
    <div class="container mx-auto py-60 pl-64">
      <p class="font-mono text-6xl text-black">C0NTACT</p>
      <p class="font-mono text-purple-800 text-base pt-10">
        E-Mail <br />
        <a
          class="font-mono text-black text-base pt-5"
          href="mailto:szymonb0106@gmail.com"
        >
          szymonb0106@gmail.com</a
        >
      </p>
      <p class="font-mono text-purple-800 text-base pt-10">
        Phone <br />
        <a class="font-mono text-black text-base pt-5" href="tel:+48721235439">
          +48 721-235-439</a
        >
      </p>
      <p class="font-mono text-purple-800 text-base pt-10">
        Dm <br />
        <a
          class="font-mono text-black text-base pt-5"
          href="https://www.messenger.com/t/piekielniedlugikurak"
        >
          messenger.com</a
        >
      </p>
    </div>
    <div class="grid grid-cols-3 pt-6"></div>
  </div>
  <div class="h-24 bg-white border-t-2 border-black sticky top-0">
    <p class="font-mono text-black text-base pt-10 pl-10">
      Made with 💜 by
      <a class="font-mono text-purple-800 text-base" href="https://szymonb.pl">
        szymonb_</a
      >
    </p>
  </div>
</template>

<script></script>
