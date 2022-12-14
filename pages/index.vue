<template>
  <div class="bg-nord2">
    <NavBar />
    <div class="flex flex-col">
      <div class="flex flex-col ml-[15%] mr-[15%] mt-[18rem] mb-[10rem] items-center bg-nord8 rounded-3xl shadow-lg">
        <vue-typer
          class="font-mono text-6xl font-semibold mt-[2rem] mb-[2rem]"
          text="Joshua Viszlai"
          :repeat="0"
          type-delay="100"
          pre-type-delay="500"
        ></vue-typer>
      </div>
      <a name="about" class="flex flex-col ml-[15%] mr-[15%] mb-[10rem] bg-nord8 rounded-3xl shadow-md shadow-nord11">
        <div class="font-mono text-5xl text-nord2 font-semibold mt-[1rem] ml-[2rem]"> About </div>
        <div> <hr class="border-nord11 border-2 shadow-lg"> </div>
        <div class="font-sans text-xl text-nord2 mt-[1rem] ml-[2rem] mr-[2rem] mb-[1rem]">
          Hi! I'm Joshua Viszlai, a Computer Science PhD student at the University of Chicago advised by <a href="https://people.cs.uchicago.edu/~ftchong/" class="text-nord11"><u>Prof. Fred Chong</u></a>. I previously completed my B.S. in Computer Science and minor in Physics at Georgia Tech. <br><br>
          My research aims to bridge the gap between current quantum devices and fault-tolerant quantum computation. I'm primarily focused on designing quantum error correction schemes in the context of today's physical systems. Although I'm also interested in quantum algorithms and near-term applications of quantum computers. My work is a part of <a href="https://www.epiqc.cs.uchicago.edu/" class="text-nord11"><u>EPiQC</u></a> (Enabling Practical-scale Quantum Computation), an NSF Expedition in Computing. Previously at Georgia Tech I worked on classical compilers, computer architecture, and robotics.
        </div>
      </a>
       <a name="publications" class="flex flex-col ml-[15%] mr-[15%] mb-[10rem] bg-nord8 rounded-3xl shadow-md shadow-nord12">
        <div class="font-mono text-5xl text-nord2 font-semibold mt-[1rem] ml-[2rem]"> Publications </div>
        <div> <hr class="border-nord12 border-2 shadow-lg"> </div>
        <ul class="list-disc font-sans text-xl text-nord2 mt-[1rem] ml-[2rem] mr-[2rem] mb-[1rem]">
          <li>
            <b>Training Quantum Boltzmann Machines with Coresets</b><br>
            <span class="text-nord12">Joshua Viszlai</span>, Teague Tomesh, Pranav Gokhale, Eric Anschuetz, Fred Chong<br>
            <i>IEEE International Conference on Quantum Computing and Engineering (QCE 22)</i>
          </li>
          <br>
          <li>
            <b>SupermarQ: A Scalable Quantum Benchmark Suite</b>(<a href="https://arxiv.org/abs/2202.11045" class="text-nord12"><u>arXiv</u></a>) <b class="text-nord11"> Best Paper Award</b><br>
            Teague Tomesh, Pranav Gokhale, Victory Omole, Gokul Subramanian Ravi, Kaitlin Smith, <span class="text-nord12">Joshua Viszlai</span>, Xin-Chuan Wu, Nikos Hardavellas, Margaret R. Martonosi, Fred Chong<br>
            <i>The 28th IEEE International Symposium on High-Performance Computer Architecture (HPCA-28)</i>
          </li>
          <br>
          <li>
            <b>Adapting Quantum Approximation Optimization Algorithm (QAOA) for Unit Commitment</b> (<a href="https://arxiv.org/abs/2110.12624" class="text-nord12"><u>arXiv</u></a>)<br>
            Samantha Koretsky, Pranav Gokhale, Jonathan M. Baker, <span class="text-nord12">Joshua Viszlai</span>, Honghao Zheng, Niroj Gurung, Ryan Burg, Esa Aleksi Paaso, Amin Khodaei, Rozhin Eskandarpour, Fred Chong<br>
            <i>IEEE International Conference on Quantum Computing and Engineering (QCE 21)</i>
          </li>
        </ul>
      </a>
      <a name="teaching" class="flex flex-col ml-[15%] mr-[15%] mb-[10rem] bg-nord8 rounded-3xl shadow-md shadow-nord13">
        <div class="font-mono text-5xl text-nord2 font-semibold mt-[1rem] ml-[2rem]"> Teaching </div>
        <div> <hr class="border-nord13 border-2 shadow-lg"> </div>
        <ul class="list-disc font-sans text-xl text-nord2 mt-[1rem] ml-[2rem] mr-[2rem] mb-[1rem]">
          <li>
            Teaching Assistant for UChicago's CMSC32900 - Quantum Computer Systems
            <span style="float:right">(Spring 2022)</span>
          </li>
          <li>
            Teaching Assistant for UChicagoX's Quantum Computer Systems Design
            <span style="float:right">(Fall 2021 - Present)</span>
          </li>
          <li>
            Computer Science Instuctor for Georgia Governor's Honors Program
            <span style="float:right">(Summer 2021)</span>
          </li>         
          <li>
            Georgia Tech's CS2110 - Computer Organization and Programming <br>
            <ul class="list-[square] font-sans ml-[2rem]">
              <li>Head Teaching Assistant <span style="float:right">(Fall 2019 - Spring 2020)</span></li>
              <li>Teaching Assistant <span style="float:right">(Spring 2018 - Spring 2019)</span></li>
            </ul>
          </li>
        </ul>
      </a>
    </div>
  </div>
</template>

<script lang="ts">
import NavBar from "@/components/NavBar.vue";

export default {
  components: {
    NavBar,
  },
};
</script>

<style lang="scss">
.vue-typer {
  /* Styles for the vue-typer container
     e.g. font-family, font-size  */

  .custom.char {
    /* Styles for each character
       e.g. color, background-color */
    color: rgb(59, 66, 82);
  }

  .custom.caret {
    /* Styles for the caret
       e.g. background-color, animation, display */

    background-color: rgb(236, 239, 244);
    width: 1rem;

     &.pre-type {
      /* Styles for the caret when it is idle before typing
         i.e. before a string starts being typed, during 'preTypeDelay' */
        background-color: transparent;
    }
  }
}
</style>
