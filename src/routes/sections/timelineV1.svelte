<script>
  import Card from "./card.svelte";
  export let date ="";
</script>

<div class="container">
  <div class="flex flex-col md:grid grid-cols-12 mb-2">
    <div class="flex md:contents">
      <p
        class="col-start-1 col-end-1 self-center text-right text-sm text-gray-400"
      >
        Dec 2023
      </p>
      <div class="col-start-2 col-end-2 mr-10 md:mx-auto relative">
        <div class="h-full w-6 flex items-center justify-center">
          <div
            class="h-full border-l-[3px] border-dotted pointer-events-none"
          ></div>
        </div>
        <div
          class="w-6 h-6 absolute top-1/2 -mt-3 rounded-full bg-white shadow border-blue-500 border-4 text-center flex items-center justify-center"
        ></div>
        <i class="fa-solid fa-chevron-up absolute left-1 text-gray-300"></i>
      </div>
      <div
        class="bg-white-500 col-start-3 col-end-10 my-4 mr-auto w-full flex gap-8"
      >
        <Card
          imgUrl="steve.jpg"
          text="No amount of technology can convert a bad story into a good story."
        />
        <Card
          imgUrl="sam.webp"
          text="No amount of technology can convert a bad story into a good story."
        />
      </div>
    </div>
  </div>
</div>
