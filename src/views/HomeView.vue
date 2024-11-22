<script setup lang="ts">
const projects = [
  {
    title: "IoT Water Quality Monitoring",
    description:
      "A water quality monitoring system using IoT leverages sensors, microcontrollers, and cloud services to collect and display data on various water parameters.",
    link: "https://github.com/ikhsanurasidb/water-quality-monitoring-final",
    image: "portfolio-1.png",
  },
  {
    title: "Simple CRUD and Pagination using Spring Boot and Vue.js",
    description:
      "A blog application created with Laravel to manage posts and user authentication.",
    link: "https://github.com/ikhsanurasidb/Simple-CRUD-Pagination-SpringBoot-VueJs",
    image: "",
  },
  {
    title: "Real-Time Traffic Monitoring YOLOv8",
    description:
      "Real-Time object detection application for traffic monitoring, Detect vehicles including cars, motorbikes, buses, and trucks. In the absence of an IP camera, a custom RTSP server is utilized to simulate the transmission of real-time video. RTSP, a standard protocol, is used for streaming video data from IP cameras.",
    link: "https://github.com/ikhsanurasidb/Real-Time-Traffic-Monitoring-YOLOv8",
    image: "portfolio-3.png",
  },
  {
    title: "Camera Location",
    description:
      "A simple Android gallery app to take pictures and get your last location for your photo details",
    link: "https://github.com/ikhsanurasidb/Camera-Location",
    image: "portfolio-4.jpeg",
  },
  {
    title: "Artistique",
    description:
      "Artistique is a web platform designed for buying and selling artwork. It includes a live auction feature, allowing users to bid on artworks in real time.",
    link: "https://github.com/ikhsanurasidb/artistique",
    image: "portfolio-5.png",
  },
];
</script>

<template>
  <main>
    <section class="flex justify-around text-center">
      <figure class="">
        <img
          src="../assets/programmer.svg"
          alt="Muhammad Ikhsan Nurasid"
          class=""
        />
      </figure>
      <article class="flex flex-col justify-center items-center w-[35dvw]">
        <h1 class="self-start text-4xl font-bold">Hello, there!</h1>
        <p class="mt-4 text-lg text-justify indent-16">
          My name is Muhammad Ikhsan Nurasid, a Computer Science student at
          Binus Bandung University with a passion for technology and innovation.
          Throughout my academic journey, I've honed my skills in backend
          development using Java, Spring Boot, and PostgreSQL. I also have a
          good foundation in HTML/CSS/JS and Vue.js for web development, while
          also diving into the exciting world of IoT. I'm passionate about
          creating innovative solutions, exploring cutting-edge technology, and
          turning ideas into impactful projects. Welcome to my portfolio—feel
          free to explore and get a glimpse of my journey as a developer! 🚀
        </p>
      </article>
    </section>

    <section id="about" class="mt-8">
      <h2 class="mb-4 text-2xl font-bold">About Me</h2>
      <div class="flex flex-col items-start justify-between md:flex-row">
        <!-- Education -->
        <div class="w-full md:w-1/2">
          <h3 class="mb-2 text-lg font-semibold">Education</h3>
          <div class="pl-4 border-l-4 border-blue-500">
            <div class="mb-4">
              <h4 class="font-bold">Binus Bandung University</h4>
              <p class="text-sm italic">Bachelor in Computer Science</p>
              <p class="text-sm">2022 - Present</p>
              <div class="flex flex-wrap gap-2 mt-2">
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Data Structures</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Database</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded">OOP</span>
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Comp Networks</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Software Eng</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >IoT Development & Architecture</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Web Development</span
                >
              </div>
            </div>
          </div>
        </div>
        <!-- Experiences -->
        <div class="w-full mt-8 md:w-1/2 md:mt-0">
          <h3 class="mb-2 text-lg font-semibold">Experiences</h3>
          <div class="pl-4 border-l-4 border-green-500">
            <div class="mb-4">
              <h4 class="font-bold">IoT Research Assistant</h4>
              <p class="text-sm italic">Water Quality Monitoring System</p>
              <p class="text-sm">2023 - 2024</p>
              <div class="flex flex-wrap gap-2 mt-2">
                <span class="px-2 py-1 text-sm bg-gray-200 rounded">IoT</span>
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >AWS IoT</span
                >
                <span class="px-2 py-1 text-sm bg-gray-200 rounded">MQTT</span>
                <span class="px-2 py-1 text-sm bg-gray-200 rounded"
                  >Arduino/ESP</span
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="projects" class="mt-8">
      <h2 class="text-2xl font-bold">Projects</h2>
      <p class="mt-4 text-lg">Here are some of my projects:</p>
      <div class="grid grid-cols-1 gap-8 mt-4 md:grid-cols-2 lg:grid-cols-3">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="overflow-hidden transition-shadow duration-300 border rounded-lg shadow-md hover:shadow-lg"
        >
          <img
            :src="project.image"
            :alt="project.title"
            class="object-cover w-full h-48"
          />
          <div class="p-4">
            <h3 class="text-xl font-bold">{{ project.title }}</h3>
            <p class="mt-2 text-gray-600">{{ project.description }}</p>
            <a
              :href="project.link"
              target="_blank"
              class="inline-block px-4 py-2 mt-4 text-white bg-blue-500 rounded hover:bg-blue-600"
            >
              View on GitHub
            </a>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" class="mt-8">
      <h2 class="text-2xl font-bold">Contact</h2>
      <p class="mt-4 text-lg">
        You can reach me via email at
        <a href="mailto:muhammad.nurasid@binus.ac.id" class="text-blue-400"
          >muhammad.nurasid@binus.ac.id</a
        >
      </p>
    </section>

    <section id="social-media" class="mt-8">
      <h2 class="text-2xl font-bold">Social Media</h2>
      <ul class="mt-4">
        <li class="text-lg">
          <a href="https://www.instagram.com/bcdefghikhsan" class="text-blue-400">Instagram</a>
        </li>
        <li class="text-lg">
          <a href="https://www.linkedin.com/in/muhammad-ikhsan-nurasid-847104226/" class="text-blue-400">LinkedIn</a>
        </li>
      </ul>
    </section>
  </main>
</template>
