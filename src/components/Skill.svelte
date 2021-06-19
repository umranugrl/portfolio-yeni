<script>
  export let baslik;
  export let oran;
</script>

<div class="mb-3">
  <div class="w-full">
    {baslik}
  </div>
  <div class="oran w-full box-border">
    <div class="oran-dolum" style={`width: ${oran}%;`} />
  </div>
</div>

<style>
  .oran {
    background-color: transparent;
    border: 2px solid #9bd952;
    height: 19px;
    border-radius: 9px;
    padding: 0;
  }
  .oran-dolum {
    border: 1px solid #fff;
    background-color: #9bd952;
    border-radius: 7px;
    height: 15px;
  }
</style>
