<script>
  import { goto } from "$app/navigation";
  import "../app.css";
</script>

<!-- Navbar -->
<div class="bg-base-100 justify-between fixed top-0 left-0 right-0">
  <div class="navbar max-w-3xl mx-auto justify-between">
    <!-- left side of navbar-->
    <div>
      <a href="/" class="btn btn-ghost text-xl">PokePage</a>
      <a href="/user" class="btn btn-ghost text-xl">My Page</a>
    </div>
    <!-- right side of navbar-->
    <div>
      <button on:click={() => goto("/login")}>Login</button>
      <span class="text-white text-lg ml-2">CJPizzle</span>
      <button on:click={() => console.log("logging out")}>Logout</button>
    </div>
  </div>
</div>

<slot></slot>
