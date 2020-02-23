<template>
  <div>
    <h1>mini msg: {{miniMsg}}</h1>
    <h2>mini data: {{foo}}</h2>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Watch, Vue } from 'vue-property-decorator';

@Component
export default class Mini extends Vue {
  @Prop() private readonly miniMsg!: string;
  foo = new Date();

  @Watch('miniMsg')
  onMiniMsgChanged(val: string, oldVal: string) {
    console.info(val, oldVal);
  }

  updateFoo() {
    this.foo = new Date();
  }
}
</script>

<style />
