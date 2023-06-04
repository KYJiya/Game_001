<script>
  import Router from 'svelte-spa-router'
  import Hello from "./routes/Hello.svelte"
  import Navigation from "./components/Navigation.svelte"
  import UserCreate from "./routes/UserCreate.svelte"
  import UserLogin from "./routes/UserLogin.svelte"

  const routes = {
    '/': Hello,
    '/user-create': UserCreate,
    '/user-login': UserLogin,
  }
</script>

<Navigation />
<Router {routes}/>