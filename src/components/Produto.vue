<template>
  <div class="bla">
    <Scene>
      <Camera type="arcRotate" :radius="7.5" :beta="Math.PI / 3"></Camera>
      <HemisphericLight></HemisphericLight>
      <Asset
        src="../assets/images/shirt.obj"
        :scaling="[7.5, 7.5, 7.5]"
        :position="[-4, -0.25, -0.5]"
        :rotation="[0, Math.PI, 0]"
      ></Asset>
     <!--  <Asset
        src="https://www.babylonjs-playground.com/scenes/skull.babylon"
        :scaling="[0.02, 0.02, 0.02]"
        :position="[4, 0.5, 0]"
      ></Asset>
      <h1>Textao</h1>
      <Asset
        src="https://www.babylonjs-playground.com/scenes/StanfordBunny.obj"
        :scaling="[7.5, 7.5, 7.5]"
        :position="[-4, -0.25, -0.5]"
        :rotation="[0, Math.PI, 0]"
      ></Asset>
      <Asset
        src="https://rawgit.com/saswata26/misc/master/base.stl"
        :scaling="[0.02, 0.02, 0.02]"
        :position="[-2, 0, -0.5]"
      ></Asset> -->
    </Scene>
  </div>
</template>
<script>
import { Entity, Scene, Camera, HemisphericLight, Asset } from "vue-babylonjs";
export default {
  mixins: [Entity],
  components: { Scene, Camera, HemisphericLight, Asset },
};
</script>