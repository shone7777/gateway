<script lang="ts">
  import * as Card from "$lib/components/ui/card";
  import { Button } from "$lib/components/ui/button";
  import { Input } from "$lib/components/ui/input";
  import { Label } from "$lib/components/ui/label";

  function handleSubmit() {
    // Redirect to the desired page
    window.location.href = "./loggedin";
  }
</script>

<div class="container flex justify-center items-center h-screen">
  <Card.Root class="w-[350px] p-6 bg-gray-100 rounded-lg shadow-lg">
    <Card.Header class="space-y-1 flex justify-center items-center h-[80px]">
      <Card.Title class="text-center text-2xl font-semibold">Login</Card.Title>
    </Card.Header>
    <Card.Content class="grid gap-4">
      <div class="grid gap-2">
        <Label for="username" class="text-gray-600">Username</Label>
        <Input
          id="username"
          type="text"
          placeholder="Username"
          class="border border-gray-300 px-3 py-2 rounded-md focus:outline-none focus:border-blue-400"
        />
      </div>
      <div class="grid gap-2">
        <Label for="password" class="text-gray-600">Password</Label>
        <Input
          id="password"
          type="password"
          class="border border-gray-300 px-3 py-2 rounded-md focus:outline-none focus:border-blue-400"
        />
      </div>
    </Card.Content>
    <Card.Footer class="mt-4">
      <Button
        on:click={handleSubmit}
        class="w-full bg-blue-500 text-white py-2 px-4 rounded-md hover:bg-blue-600 transition duration-300"
        >Submit</Button
      >
    </Card.Footer>
  </Card.Root>
</div>
