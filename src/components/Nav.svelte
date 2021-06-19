<script>
  export let segment;

  import successkid from "images/successkid.jpg";
</script>

<nav
  class="w-full flex justify-center items-center flex-nowrap md:hidden bg-gray-200"
>
  <img class="rounded-full w-2/12" src={successkid} alt="Ümran Uğurlu" />
  <ul>
    <li>
      <a aria-current={segment === undefined ? "page" : undefined} href="."
        >Anasayfa</a
      >
    </li>
    <li>
      <a
        aria-current={segment === "about-me" ? "page" : undefined}
        href="about-me">Hakkımda</a
      >
    </li>
    <li>
      <a
        aria-current={segment === "education" ? "page" : undefined}
        href="education">Eğitim</a
      >
    </li>
    <li>
      <a
        aria-current={segment === "experience" ? "page" : undefined}
        href="experience">Deneyim</a
      >
    </li>
  </ul>
</nav>

<style>
  nav {
    border-bottom: 1px solid rgba(255, 62, 0, 0.1);
    font-weight: 300;
    padding: 0 1em;
  }

  ul {
    margin: 0;
    padding: 0;
  }

  ul::after {
    content: "";
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: left;
  }

  [aria-current] {
    position: relative;
    display: inline-block;
  }

  [aria-current]::after {
    position: absolute;
    content: "";
    width: calc(100% - 1em);
    height: 2px;
    background-color: #7cb900;
    display: block;
    bottom: -1px;
  }

  a {
    text-decoration: none;
    padding: 1em 0.5em;
    display: block;
  }
</style>
