<script lang="ts">
  //import Activity from "lucide-svelte/icons/activity";
  //import CreditCard from "lucide-svelte/icons/credit-card";
  //import DollarSign from "lucide-svelte/icons/dollar-sign";
  // import Download from "lucide-svelte/icons/download";
  //import Users from "lucide-svelte/icons/users";
  import { Button } from "../lib/components/ui/button";
  import * as Card from "../lib/components/ui/card/index";
  // import * as Tabs from "$lib/registry/new-york/ui/tabs/index.js";
  import Overview from "../../src/overview.svelte";
  import RecentSales from "../lib/components/dashboard/connecteddevice.svelte";
  //import DatePickerWithRange from "$lib/registry/new-york/example/date-picker-with-range.svelte";
  //import DashboardLight from "$lib/img/examples/dashboard-light.png";
  //import DashboardDark from "$lib/img/examples/dashboard-dark.png";
</script>

<div class="hidden flex-col md:flex">
  <div class="border-b"></div>
  <div class="flex-1 space-y-4 p-8 pt-6">
    <div class="flex items-center justify-between space-y-2">
      <h2 class="text-3xl font-bold tracking-tight">User Details</h2>
    </div>

    <div class="grid gap-4 md:grid-cols-2 lg:grid-cols-4"></div>
    <div class="grid gap-4 md:grid-cols-2 lg:grid-cols-7">
      <Card.Root class="col-span-4">
        <Card.Header>
          <Card.Title>Data Usage</Card.Title>
        </Card.Header>
        <Card.Content>
          <Overview />
        </Card.Content>
      </Card.Root>
      <Card.Root class="col-span-3">
        <Card.Header>
          <Card.Title>Connected Devices</Card.Title>
        </Card.Header>
        <Card.Content>
          <RecentSales />
        </Card.Content>
      </Card.Root>
    </div>
  </div>
</div>
