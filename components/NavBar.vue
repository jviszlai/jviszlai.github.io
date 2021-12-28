<template>
  <div class="flex flex-row-reverse items-center overflow-clip fixed right-0">
    <div
      class="flex flex-row items-center justify-evenly bg-nord8 shadow-lg rounded-md m-1 mr-0 w-[16rem] z-10"
    >
      <a href="mailto:viszlai@uchicago.edu"
        ><font-awesome-icon
          :icon="['fas', 'envelope']"
          class="text-4xl text-nord2 hover:text-nord6 m-2 transition-colors"
        />
      </a>
      <a href="https://github.com/jviszlai"
        ><font-awesome-icon
          :icon="['fab', 'github']"
          class="text-4xl text-nord2 hover:text-nord6 m-2 transition-colors"
        />
      </a>
      <a href="https://www.linkedin.com/in/joshua-viszlai-909797144"
        ><font-awesome-icon
          :icon="['fab', 'linkedin']"
          class="text-4xl text-nord2 hover:text-nord6 m-2 transition-colors"
        />
      </a>
      <a href="#"
        ><font-awesome-icon
          :icon="['fas', 'file-alt']"
          class="text-4xl text-nord2 hover:text-nord6 m-2 transition-colors"
        />
      </a>
      <a href="https://jviszlai.github.io/gba/"
        ><font-awesome-icon
          :icon="['fas', 'gamepad']"
          class="text-4xl text-nord2 hover:text-nord6 ml-2 mr-2 transition-colors"
        />
      </a>
    </div>
    <div
      class="flex flex-row items-center text-nord2 bg-nord5 text-2xl shadow-lg rounded-2xl bg-opacity-75 w-[32rem] h-3/4 relative -right-[29.5rem] hover:-right-[8rem] transition-all duration-[1500ms] z-0"
    >
      <font-awesome-icon
        :icon="['fas', 'ellipsis-h']"
        class="ml-3 mt-2 mb-2 mr-1"
      />
      <a
        href="#about"
        class="ml-2 mr-2 text-xl font-mono font-medium hover:bg-nord8 transition-colors rounded-lg"
        >About</a
      >
      <a
        href="#publications"
        class="ml-2 mr-2 text-xl font-mono font-medium hover:bg-nord8 transition-colors rounded-lg"
        >Publications</a
      >
      <a
        href="#teaching"
        class="ml-2 mr-2 text-xl font-mono font-medium hover:bg-nord8 transition-colors rounded-lg"
        >Teaching</a
      >
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
