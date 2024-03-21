<!-- App.svelte -->
<script>
  import { Route, Router } from "svelte-routing";
  import login from "./loggedin.svelte";
  import signUp from "./signup.svelte";
  import user from "../src/dash2/hello.svelte";
</script>

<Router>
  <Route path="/" component={login} />
  <Route path="/signup" component={signUp} />
  <Route path="/user" component={user} />
</Router>
