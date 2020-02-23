<template>
  <div class="hello">
    <h3>todo: {{ todo }}</h3>
    <h2>aa {{ reverse }}</h2>
    <button @click="updateSome">aa {{ some }}</button>
    <input type="submit" :value="msg">
    <h1>{{ msg }}</h1>
    <Mini miniMsg="something message" ref="minimini" />
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-typescript" target="_blank" rel="noopener">typescript</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-router" target="_blank" rel="noopener">router</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-unit-jest" target="_blank" rel="noopener">unit-jest</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Watch, Ref, Vue } from 'vue-property-decorator';
import Mini from './MiniComponent.vue';

@Component({
  components: {
    Mini
  }
})
export default class HelloWorld extends Vue {
  some: string | null = null;
  todoId = 1;
  todo: object = {};

  @Prop() private readonly msg!: string;

  @Ref() private readonly minimini?: Mini;

  @Watch('some')
  onSomeChanged(val: string, oldVal: string) {
    console.info(val, oldVal);
  }

  @Watch('todoId')
  onTodoIdChanged(val: number, oldVal: number) {
    console.info(val, oldVal);
    fetch(`https://jsonplaceholder.typicode.com/todos/${this.todoId}`)
    .then((resolve) => resolve.json())
    .then((resolve) => this.todo = resolve)
    .catch((reject) => console.info(reject))
    .finally();
  }

  get reverse() {
    return this.msg.split("").reverse().join("") + " " + this.some?.split("").reverse().join("");
  }

  updateSome() {
    console.log("a:", this.some);
    this.some = "some";
    console.info("clicked");
    this.todoId++;

    this.minimini?.updateFoo();
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
