<template>
  <!-- We use viewport height + aspect ratio to define width for container that 
    holds everything, AKA app container -->
  <main
    class="flex flex-wrap flex-col justify-center landscape:items-center landscape:max-xl:max-w-[1200px] landscape:xl:mx-auto"
  >
    <!-- This creates the container that sets the main container width -->
    <div
      class="landscape:h-[80vh] landscape:aspect-video relative portait:w-full"
    >
      <!-- This is where the video goes, it pins absolute to the created container -->
      <!-- Focus on the positioning only, the rest is for create item reference -->
      <section
        class="flex items-center justify-center bg-red-700 absolute landscape:inset-0 portrait:inset-x-0"
      >
        <!-- Video.js player when set to 16:9 aspect ratio will always return that aspect ratio -->
        <!-- We just need set this container to 100% width -->
        <!-- The height will be autofill -->
        <div class="w-full">
          <video
            id="my-video"
            class="video-js vjs-fluid"
            controls
            preload="auto"
            data-setup="{}"
          >
            <source
              src="http://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4"
              type="video/mp4"
            />
            <p class="vjs-no-js">
              To view this video please enable JavaScript, and consider
              upgrading to a web browser that
              <a href="https://videojs.com/html5-video-support/" target="_blank"
                >supports HTML5 video</a
              >
            </p>
          </video>
        </div>
      </section>

      <!-- Quest Description: Warmup Etc -->
      <section class="bg-pink-400 w-full pt-[56.25%]">
        <div class="flex items-center p-4">
          <section class="w-2/3">
            <h1 class="text-3xl">Program Header Description</h1>
          </section>
          <section class="w-1/3">
            <button class="rounded bg-blue-400 px-4 py-2">Button</button>
          </section>
        </div>
      </section>

      <!-- Lesson Items -->
      <section class="bg-green-400 w-full">
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
        <div class="w-full h-32">
          <h2 class="text-2xl">Item</h2>
        </div>
      </section>
    </div>
  </main>
</template>
