<script>
  import { Button } from "$lib/components/ui/button";
  import * as DropdownMenu from "$lib/components/ui/dropdown-menu";
  import * as Avatar from "$lib/components/ui/avatar";
</script>

<header class="flex flex-col relative z-20">
  <div
    class="max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6 border-dotted border-b-[3px]"
  >
    <a class="flex items-center gap-1 font-semibold text-xl" href="/"
      ><img src="/icons/logo-main.svg" alt="" /> <span>duggup</span></a
    >
    <button class="md:hidden grid place-items-center">
      <i class="fa-solid fa-bars"></i>
    </button>
    <nav class="hidden md:flex items-center gap-12 sm:hidden">
      <a class="flex items-center gap-3 hover:text-brand-primary" href="/"
        ><img src="/icons/home.svg" alt="" /> Home</a
      >
      <a class="flex items-center gap-3 hover:text-brand-primary" href="/"
        ><img src="/icons/explore.svg" alt="" /> Explore</a
      >
      <a class="flex items-center gap-3 hover:text-brand-primary" href="/"
        ><img src="/icons/book.svg" alt="" /> Learn</a
      >
      <Button variant="cta" class="flex gap-2"
        ><i class="fa-regular fa-square-plus"></i> Button</Button
      >
      <DropdownMenu.Root>
        <DropdownMenu.Trigger class="flex items-center gap-2">
          <Avatar.Root>
            <Avatar.Image src="/profile.png" alt="@shadcn" />
            <Avatar.Fallback>CN</Avatar.Fallback>
          </Avatar.Root>
          <span>Krishna Kiran</span>
        </DropdownMenu.Trigger>
        <DropdownMenu.Content>
          <DropdownMenu.Group>
            <DropdownMenu.Label>My Account</DropdownMenu.Label>
            <DropdownMenu.Separator />
            <DropdownMenu.Item>Profile</DropdownMenu.Item>
            <DropdownMenu.Item>Billing</DropdownMenu.Item>
            <DropdownMenu.Item>Team</DropdownMenu.Item>
            <DropdownMenu.Item>Subscription</DropdownMenu.Item>
          </DropdownMenu.Group>
        </DropdownMenu.Content>
      </DropdownMenu.Root>
    </nav>
  </div>
</header>
