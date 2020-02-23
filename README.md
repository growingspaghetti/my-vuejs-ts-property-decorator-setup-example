# vue-ts-practice

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your unit tests
```
npm run test:unit
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

# install manual
<pre><font color="#A6E22E"><b>ryoji@ubuntu</b></font>:<font color="#66D9EF"><b>~/dev</b></font>$ vue create vue-ts-practice


<font color="#66D9EF"><b>Vue CLI v4.2.2</b></font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Please pick a preset:</b></font> <font color="#A1EFE4">Manually select features</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Check the features needed for your project:</b></font> 
 <font color="#A6E22E">◉</font> Babel
 <font color="#A6E22E">◉</font> TypeScript
 ◯ Progressive Web App (PWA) Support
 <font color="#A6E22E">◉</font> Router
 <font color="#A6E22E">◉</font> Vuex
 ◯ CSS Pre-processors
 <font color="#A6E22E">◉</font> Linter / Formatter
<font color="#A1EFE4">❯</font><font color="#A6E22E">◉</font><font color="#A1EFE4"> Unit Testing</font>
 ◯ E2E Testing

</pre>

---

<pre><font color="#A6E22E"><b>ryoji@ubuntu</b></font>:<font color="#66D9EF"><b>~/dev</b></font>$ vue create vue-ts-practice


<font color="#66D9EF"><b>Vue CLI v4.2.2</b></font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Please pick a preset:</b></font> <font color="#A1EFE4">Manually select features</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Check the features needed for your project:</b></font> <font color="#A1EFE4">Babel, TS, Router, Vuex, CSS Pre-processors, Linter, Unit</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Use class-style component syntax?</b></font> <font color="#A1EFE4">Yes</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Use Babel alongside TypeScript (required for modern mode, auto-detected polyfills, transpiling JSX)?</b></font> <font color="#A1EFE4">Yes</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Use history mode for router? </b></font><font color="#F4BF75"><b>(Requires proper server setup for index fallback in production)</b></font> <font color="#A1EFE4">No</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default):</b></font> <font color="#A1EFE4">Sass/SCSS (with dart-sass)</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Pick a linter / formatter config:</b></font> <font color="#A1EFE4">Basic</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Pick additional lint features:</b></font> (Press <font color="#A1EFE4"><b>&lt;space&gt;</b></font> to select, <font color="#A1EFE4"><b>&lt;a&gt;</b></font> to toggle all, <font color="#A1EFE4"><b>&lt;i&gt;</b></font> to invert selection)<font color="#A1EFE4">Lint on save</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Pick a unit testing solution:</b></font> <font color="#A1EFE4">Jest</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Where do you prefer placing config for Babel, ESLint, etc.?</b></font> <font color="#A1EFE4">In dedicated config files</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Save this as a preset for future projects?</b></font> <font color="#A1EFE4">Yes</font>
<font color="#A6E22E">?</font> <font color="#F8F8F2"><b>Save preset as:</b></font> <font color="#A1EFE4">typescript-scss</font>


<font color="#66D9EF"><b>Vue CLI v4.2.2</b></font>
✨  Creating project in <font color="#F4BF75">/media/dev/vue-ts-practice</font>.
🗃  Initializing git repository...
⚙️  Installing CLI plugins. This might take a while...


&gt; yorkie@2.0.0 install /media/dev/vue-ts-practice/node_modules/yorkie
&gt; node bin/install.js

setting up Git hooks
done


&gt; core-js@2.6.11 postinstall /media/dev/vue-ts-practice/node_modules/babel-runtime/node_modules/core-js
&gt; node -e &quot;try{require(&apos;./postinstall&apos;)}catch(e){}&quot;


&gt; core-js@3.6.4 postinstall /media/dev/vue-ts-practice/node_modules/core-js
&gt; node -e &quot;try{require(&apos;./postinstall&apos;)}catch(e){}&quot;


&gt; ejs@2.7.4 postinstall /media/dev/vue-ts-practice/node_modules/ejs
&gt; node ./postinstall.js

added 1427 packages from 1058 contributors and audited 935171 packages in 34.409s

36 packages are looking for funding
  run `npm fund` for details

found <font color="#A6E22E">0</font> vulnerabilities

🚀  Invoking generators...
📦  Installing additional dependencies...

added 77 packages from 38 contributors and audited 937716 packages in 18.213s

43 packages are looking for funding
  run `npm fund` for details

found <font color="#A6E22E">0</font> vulnerabilities

⚓  Running completion hooks...

📄  Generating README.md...

🎉  Successfully created project <font color="#F4BF75">vue-ts-practice</font>.
👉  Get started with the following commands:

<font color="#A1EFE4"> </font><font color="#75715E">$</font><font color="#A1EFE4"> cd vue-ts-practice</font>
<font color="#A1EFE4"> </font><font color="#75715E">$</font><font color="#A1EFE4"> npm run serve</font>
</pre>

# test:unit
<pre><font color="#A6E22E"><b>ryoji@ubuntu</b></font>:<font color="#66D9EF"><b>~/dev/vue-ts-practice</b></font>$ npm run test:unit

&gt; vue-ts-practice@0.1.0 test:unit /media/dev/vue-ts-practice
&gt; vue-cli-service test:unit

<span style="background-color:#A6E22E"><font color="#272822"><b> PASS </b></font></span> tests/unit/<font color="#F8F8F2"><b>example.spec.ts</b></font>
  HelloWorld.vue
    <font color="#A6E22E">✓</font> renders props.msg when passed (25ms)

<font color="#F8F8F2"><b>Test Suites: </b></font><font color="#A6E22E"><b>1 passed</b></font>, 1 total
<font color="#F8F8F2"><b>Tests:       </b></font><font color="#A6E22E"><b>1 passed</b></font>, 1 total
<font color="#F8F8F2"><b>Snapshots:   </b></font>0 total
<font color="#F8F8F2"><b>Time:</b></font>        2.702s
<font color="#A5A5A1">Ran all test suites.</font></pre>

# run build
<pre><font color="#A6E22E"><b>ryoji@ubuntu</b></font>:<font color="#66D9EF"><b>~/dev/vue-ts-practice</b></font>$ npm run build

&gt; vue-ts-practice@0.1.0 build /media/dev/vue-ts-practice
&gt; vue-cli-service build


<font color="#A1EFE4">⠙</font>  Building for production...Starting type checking service...
Using <font color="#F8F8F2"><b>1 worker</b></font> with <font color="#F8F8F2"><b>2048MB</b></font> memory limit
<font color="#A1EFE4">⠹</font>  Building for production...

<span style="background-color:#A6E22E"><font color="#272822"> DONE </font></span> <font color="#A6E22E">Compiled successfully in 7307ms</font>                                                                                                                <font color="#75715E">01:48:30</font>

  <font color="#A1EFE4"><b>File</b></font>                                 <font color="#A1EFE4"><b>Size</b></font>               <font color="#A1EFE4"><b>Gzipped</b></font>

  <font color="#A6E22E">dist/js/chunk-vendors.845312db.js</font>    139.08 KiB         48.12 KiB
  <font color="#A6E22E">dist/js/app.c80b1de8.js</font>              6.96 KiB           2.43 KiB
  <font color="#A6E22E">dist/js/about.865db47c.js</font>            0.44 KiB           0.31 KiB
  <font color="#66D9EF">dist/css/app.5b4febbc.css</font>            0.42 KiB           0.26 KiB

  <font color="#75715E">Images and other types of assets omitted.</font>

<span style="background-color:#A6E22E"><font color="#272822"> DONE </font></span> Build complete. The <font color="#A1EFE4">dist</font> directory is ready to be deployed.
<span style="background-color:#66D9EF"><font color="#272822"> INFO </font></span> Check out deployment instructions at <font color="#A1EFE4">https://cli.vuejs.org/guide/deployment.html</font>
</pre>

# plugins
https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue

# also yarn
<pre><font color="#A6E22E"><b>ryoji@ubuntu</b></font>:<font color="#66D9EF"><b>/media/dev/vue-ts-practice</b></font>$ yarn run test:unit
<font color="#F8F8F2"><b>yarn run v1.21.1</b></font>
<font color="#A5A5A1">$ vue-cli-service test:unit</font>
<span style="background-color:#A6E22E"><font color="#272822"><b> PASS </b></font></span> tests/unit/<font color="#F8F8F2"><b>example.spec.ts</b></font>
  HelloWorld.vue
    <font color="#A6E22E">✓</font> renders props.msg when passed (27ms)

<font color="#F8F8F2"><b>Test Suites: </b></font><font color="#A6E22E"><b>1 passed</b></font>, 1 total
<font color="#F8F8F2"><b>Tests:       </b></font><font color="#A6E22E"><b>1 passed</b></font>, 1 total
<font color="#F8F8F2"><b>Snapshots:   </b></font>0 total
<font color="#F8F8F2"><b>Time:</b></font>        1.331s, estimated 3s
<font color="#A5A5A1">Ran all test suites.</font>
Done in 2.23s.</pre>