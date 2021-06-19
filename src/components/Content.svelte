<script>
  export let title;
  import Title from "./Content/Title.svelte";
</script>

<div class="w-full h-3/4 pl-0 md:pl-r25">
  <div
    class="content w-4/5 flex justify-center items-start flex-wrap relative mx-auto mt-5 mb:mt-0 h-full p-4"
  >
    <Title {title} />

    <slot />
  </div>
</div>

<style>
  .content {
    background-color: #b5b5b5;
    padding-top: 100px;
  }
</style>
