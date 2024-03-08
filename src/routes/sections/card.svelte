<script>
  export let text = "";
  export let imgUrl = "";
</script>

<div class="w-1/2 border border-gray-200 rounded-xl">
  <div class="w-full h-40 overflow-hidden flex items-center rounded-t-xl">
    <img src={imgUrl} alt="" />
  </div>
  <p class="p-6">
    {text}
  </p>
</div>
