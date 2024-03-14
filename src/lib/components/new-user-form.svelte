<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import { Input } from "$lib/components/ui/input";
  import { Label } from "$lib/components/ui/label";

  import { cn } from "$lib/utils.js";

  let className: string | undefined | null = undefined;
  export { className as class };

  let isLoading = false;
  async function onSubmit() {
    isLoading = true;

    setTimeout(() => {
      isLoading = false;
    }, 3000);
  }
</script>

<div class={cn("grid gap-6", className)} {...$$restProps}>
  <form on:submit|preventDefault={onSubmit}>
    <div class="grid gap-2 lg:w-full justify-center sm:justify-center sm:items-center sm:h-full">

      <div class="grid gap-1">
        <Label class="sr-only" for="firstName">First Name</Label>
        <Input
          id="firstName"
          placeholder="first name"
          type="name"
          autocapitalize="none"
          autocomplete="none"
          autocorrect="off"
          disabled={isLoading}
        />
        <Label class="sr-only" for="lastName">Last Name</Label>
        <Input
          id="lastName"
          placeholder="last name"
          type="name"
          autocapitalize="none"
          autocomplete="none"
          autocorrect="off"
          disabled={isLoading}
        />
        <Label class="sr-only" for="email">Email</Label>
        <Input
          id="email"
          placeholder="email@example.com"
          type="email"
          autocapitalize="none"
          autocomplete="email"
          autocorrect="off"
          disabled={isLoading}
        />
        <Label class="sr-only" for="password">password</Label>
        <Input
          id="password"
          placeholder="password"
          type="password"
          autocapitalize="none"
          autocomplete="none"
          autocorrect="off"
          disabled={isLoading}
        />
      </div>
      <Button disabled={isLoading}>Sign up</Button>
    </div>
  </form>
</div>