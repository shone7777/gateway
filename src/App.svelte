<!-- App.svelte -->
<script>
  import { Route, Router } from 'svelte-routing';
  import login from './loggedin.svelte';
  import signUp from './signup.svelte';
</script>

<Router>
  <Route path="/" component={login} />
  <Route path="/signup" component={signUp} />
</Router>
