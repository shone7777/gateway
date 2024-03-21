<script lang="ts">
  import AvatarImgs from "../img/avatar";
  import * as Avatar from "../avatar1";
  export { default as RecentSales } from "./connecteddevice.svelte";
</script>

<div class="space-y-8">
  <div class="flex items-center">
    <Avatar.Root class="h-9 w-9">
      <Avatar.Image src={AvatarImgs[0]} alt="Avatar" />
      <Avatar.Fallback>OM</Avatar.Fallback>
    </Avatar.Root>
    <div class="ml-4 space-y-1">
      <p class="text-sm font-medium leading-none">Olivia Martin</p>
      <p class="text-sm text-muted-foreground">olivia.martin@email.com</p>
    </div>
    <div class="ml-auto font-medium">IP</div>
  </div>
  <div class="flex items-center">
    <Avatar.Root
      class="flex h-9 w-9 items-center justify-center space-y-0 border"
    >
      <Avatar.Image src={AvatarImgs[1]} alt="Avatar" />
      <Avatar.Fallback>JL</Avatar.Fallback>
    </Avatar.Root>
    <div class="ml-4 space-y-1">
      <p class="text-sm font-medium leading-none">Jackson Lee</p>
      <p class="text-sm text-muted-foreground">jackson.lee@email.com</p>
    </div>
    <div class="ml-auto font-medium">IP</div>
  </div>
  <div class="flex items-center">
    <Avatar.Root class="h-9 w-9">
      <Avatar.Image src={AvatarImgs[2]} alt="Avatar" />
      <Avatar.Fallback>IN</Avatar.Fallback>
    </Avatar.Root>
    <div class="ml-4 space-y-1">
      <p class="text-sm font-medium leading-none">Isabella Nguyen</p>
      <p class="text-sm text-muted-foreground">isabella.nguyen@email.com</p>
    </div>
    <div class="ml-auto font-medium">IP</div>
  </div>
  <div class="flex items-center">
    <Avatar.Root class="h-9 w-9">
      <Avatar.Image src={AvatarImgs[3]} alt="Avatar" />
      <Avatar.Fallback>WK</Avatar.Fallback>
    </Avatar.Root>
    <div class="ml-4 space-y-1">
      <p class="text-sm font-medium leading-none">William Kim</p>
      <p class="text-sm text-muted-foreground">will@email.com</p>
    </div>
    <div class="ml-auto font-medium">IP</div>
  </div>
  <div class="flex items-center">
    <Avatar.Root class="h-9 w-9">
      <Avatar.Image src={AvatarImgs[4]} alt="Avatar" />
      <Avatar.Fallback>SD</Avatar.Fallback>
    </Avatar.Root>
    <div class="ml-4 space-y-1">
      <p class="text-sm font-medium leading-none">Sofia Davis</p>
      <p class="text-sm text-muted-foreground">sofia.davis@email.com</p>
    </div>
    <div class="ml-auto font-medium">IP</div>
  </div>
</div>
