<script>
  import Profil from "./Header/Profil.svelte";
  import Links from "./Header/Links.svelte";
  import Socials from "./Header/Socials.svelte";

  let open = false;
  const headerClass = `hidden md:flex justify-center items-center flex-wrap box-border h-screen bg-gray-200 fixed w-1/5 left-0 top-0 static md:fixed `;
  const menuBarClasses = [`close`, `open`];
  function HeaderKontrol() {
    return (open = !open);
  }
</script>

<div
  class={open ? `open ${headerClass}` : `close ${headerClass}`}
  on:click={HeaderKontrol}
>
  <div class="w-full flex items-center justify-end md:hidden">
    <div class={open ? menuBarClasses[0] : menuBarClasses[1]}>
      <i /><i /><i />
    </div>
  </div>

  <Profil />
  <Links />
  <Socials />
</div>
