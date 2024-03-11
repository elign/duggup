<script>
  import Button from "$lib/components/ui/button/button.svelte";
  let isFollowing = false;

  function toggleFollow() {
    isFollowing = !isFollowing;
  }
</script>

<div class="grid grid-cols-12 gap-20 mb-8">
  <div class="col-start-2 col-end-4">
    <img
      class="border-gray-200 border-4 rounded-full"
      src="/profile.png"
      alt="User Profile"
    />
    <h4 class="text-center text-3xl font-semibold text-gray-500">
      Krishna Kiran
    </h4>
  </div>
  <div class="col-start-4 col-end-10 flex flex-col justify-center gap-6">
    <p>
      Co-Founder and CEO at Duggup - Social network for people in tech.
      Ex-Amazon Head of Engineering. I write hot-takes on building a business,
      shipping delightful products and accelerating product and career growth.
    </p>
    <Button on:click={toggleFollow} variant="cta" class={`max-w-24 ${isFollowing === true && "shadow-active"}`}>
      {isFollowing ? "Followed" : "Follow"}
    </Button>
  </div>
  <div class="col-start-10 col-end-12 flex flex-col items-end justify-center">
    <img src="/icons/logo-cir.svg" alt="logo" />
    <h4 class="font-semibold text-xl">Duggup</h4>
    <h5 class="text-gray-400 text-sm mb-6">Co-Founder and CEO</h5>
    <a href="/" class="flex items-center gap-2 text-gray-600">
      <span>My Website</span>
      <img src="/icons/share.svg" alt="share" />
      <i class="fa-solid fa-ellipsis fa-2xl text-gray-300 ml-3"></i>
    </a>
  </div>
</div>
