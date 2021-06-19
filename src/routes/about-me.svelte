<script>
  import successkid from "images/successkid.jpg";
  import Content from "../components/Content.svelte";
  let title = "Hakkımda";
</script>

<svelte:head>
  <title>{title} | Ümran Uğurlu</title>
</svelte:head>

<Content {title}>
  <p class="w-full md:w-2/4">
    1995 yılının Eylül ayında İstanbul'da dünyaya geldim. Liseyi Remzi Bayraktar
    Anadolu Ticaret ve Meslek Lisesi, Web tasarım bölümü olarak okudum. Lise son
    stajımı Kayışdağı Darülacezede yaptım. Daha sonra Karabük Üniversitesi,
    Safranbolu Meslek Yüksek Okulu, Bilgisayar Teknolojisi bölümünü okudum. 2.
    sınıf yaz stajımı Ottoman Creative şirketinde yaptım. Kendimi geliştirmek
    için bir kaç muhasebe yazılımı yapan şirketlerde çalıştım. Şuan Karadeniz
    Teknik Üniversitesi, Of Teknoloji Fakültesinde Yazılım Mühendisliği
    okumaktayım.
  </p>

  <img class="w-full md:w-2/4" src={successkid} alt="Ümran Uğurlu" />
</Content>

<style global>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
