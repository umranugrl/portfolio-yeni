<script>
  import Content from "../components/Content.svelte";
  import Skill from "../components/Skill.svelte";
  let title = "Eğitim";
</script>

<svelte:head>
  <title>{title} | Ümran Uğurlu</title>
</svelte:head>

<Content {title}>
  <div class="w-full md:w-2/4">
    <div class="w-full">
      <h2 class="text-bold text-2xl mb-5">Tasarım Becerileri</h2>
      <div class="w-full">
        <Skill baslik="web tasarım" oran={80} />
        <Skill baslik="grafik tasarım" oran={20} />
      </div>
    </div>
  </div>
  <div class="w-full md:w-2/4">
    <div class="w-full">
      <h2 class="text-bold text-2xl mb-5">Kodlama Becerileri</h2>
      <div class="w-full">
        <Skill baslik="html" oran={80} />
        <Skill baslik="css" oran={70} />
        <Skill baslik="javascript" oran={10} />
        <Skill baslik="php" oran={65} />
        <Skill baslik="c++" oran={99} />
        <Skill baslik="c#" oran={40} />
      </div>
    </div>
  </div>
</Content>

<style global>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
