## SUMMARY IN COMMON JS

---

<li><strong>module.exports</strong> to export function, class, and variable.</li>
<li>use <strong>const variableName = require("./path/to/file")</strong> to import function, class and variable</li>
<li>commonjs requires nodejs and npm in it</li>
<li>in index.html file, when declare a entry point doesn't have to use <strong>type="module"</strong> in <strong>script</strong> tag</li>
<li>commonjs requires webpack for module bundler</li>
<li>configure package.json file, inside script <strong>"build": "webpack"</strong>. This is necessary to generate dist folder and a entry point in it.</li>
<li>after dist folder generated, include entry point usually dist/main.js in script source inside index.html file</li>
