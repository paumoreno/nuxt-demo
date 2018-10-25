<template>
  <div class="World">
    <div class="World__phrase">Hello <img class="World__icon" src="~/assets/world.png" alt="world">!</div>


    <img src="~/assets/world_bg.png" alt="world" style="width:200px">
  </div>
</template>

<script>

</script>

<style>
.World {
  text-align: center;
  background-color: #bbdefb;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.World__phrase {
  margin-bottom: 2em;
  font-size: 2em;
}

.World__icon {
  vertical-align: middle;
}
</style>

