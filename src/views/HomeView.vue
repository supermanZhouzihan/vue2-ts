<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld :msg="test" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class HomeView extends Vue {
  data() {
    return {
      test: "",
    };
  }

  mounted() {
    console.log("组件已挂载");
    this.init(2,'test');
  }

  private init(num:number,msg:string): void {
    console.log("执行init方法");
    let a: number =12;
    a = 34;


    let com ;
    com=12

    console.log(com)

  }
}
</script>
