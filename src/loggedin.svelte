<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import UserAuthForm from "./lib/components/user-auth-form.svelte";
</script>

<div
  class="container relative h-[800px] flex-col items-center justify-center sm:grid md:grid lg:max-w-none lg:grid-cols-2 lg:px-0"
>
  <div class="lg:p-8 sm:grid">
    <div
      class="mx-auto flex w-full flex-col justify-center sm:items-center space-y-6 sm:w-[350px]"
    >
      <div class="flex flex-col space-y-2 text-center">
        <h1 class="text-2xl font-semibold tracking-tight">Login</h1>
      </div>
      <UserAuthForm />
      <a href="/signup" class="mt-4 p-3"> Don't have an account ? </a>
    </div>
  </div>
  <div
    class="relative hidden h-full flex-col bg-muted p-10 text-white dark:border-r lg:flex"
  >
    <div
      class="absolute inset-0 bg-cover h-10px"
      style="
        background-image: url(./firewall.jpg);
      "
    ></div>
    <div class="relative z-20 flex items-center text-lg font-medium">
      <!-- <Command class="mr-2 h-6 w-6" /> -->
    </div>
  </div>
</div>

<style>
  .container {
    overflow: hidden;
  }
</style>
