<script>
  export let logo = "";
  export let companyName = "";
  export let location = "";
  export let date = "";
</script>

<div class="container">
  <div class="grid grid-cols-12 gap-0">
    <div class="col-start-1 col-end-2 flex flex-col items-end text-end">
      <img src={logo} alt="logo" class="w-12 h-12 mb-1"/>
      <h3 class="font-semibold text-xl">{companyName}</h3>
      <p class="text-gray-400 text-sm">{location}</p>
      <p class="text-gray-400 text-sm">Joined</p>
      <p class="text-gray-400 text-sm">{date}</p>
    </div>
    <div class="col-start-2 col-end-2 md:mx-auto relative">
      <div class="h-full w-6 flex items-center justify-center">
        <div
          class="h-full border-l-[3px] border-dotted pointer-events-none"
        ></div>
      </div>
      <div
        class="w-6 h-6 absolute top-1/2 -mt-3 rounded-full bg-white shadow border-blue-500 border-8 text-center flex items-center justify-center"
      ></div>
    </div>
    <div
      class="bg-white col-start-3 col-end-10 self-center p-4 rounded-xl my-4 mr-auto shadow-sm w-full h-24"
    >
      <h3 class="font-semibold text-xl mb-1">Co-Founder and CEO</h3>
      <p class="leading-tight text-justify text-gray-500 text-sm">
        Full-time · Remote
      </p>
    </div>
  </div>
</div>
