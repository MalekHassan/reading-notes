## EJS template
EJS is among the most popular tempate view engines for node.js and expressjs with 4.2k stars at github and over 5.5m downloads per week at npm.

EJS simply stands for Embedded JavaScript templates, and we can use it both server-side or client-side. At this story, we’ll focus on the server-side.

### Fast development time

* Don't waste time and attention figuring out arcane new syntax because 'elegance' — or how to preprocess your data so it will actually render right.

### Simple syntax

* JavaScript code in simple, straightforward scriptlet tags. Just write JavaScript that emits the HTML you want, and get the job done!

### Speedy execution

* We all know how fast V8 and the other JavaScript runtimes have gotten. EJS caches the intermediate JS functions for fast execution.

### Easy debugging

* It's easy to debug EJS errors: your errors are plain JavaScript exceptions, with template line-numbers included.

### Active development

* EJS has a large community of active users, and the library is under active development. We're happy to answer your questions or give you help.

### Basic Syntax(Tags):
* <% 'Scriptlet' tag, for control-flow, no output
* <%= Outputs the value into the template (HTML escaped)
* <%- Outputs the unescaped value into the template
* <% if (message) { %>
```
 <h2><%= message.name %></h2>
<% } %>
```
## Partials
```
<%- include('../template/head')-%>
<body class="text-center">
<div class="cover-container d-flex w-100 h-100 p-3 mx-auto flex-column">
<%- include('../template/nav')-%>
<main role="main" class="inner cover">
<h1 class="cover-heading">MasterEJS</h1>
<p class="lead">This is a sample app to Master EJS view template engine with Expressjs and Node.js framework
</p>
<p class="lead">
<a href="https://medium.com/@pkoulianos/master-ejs-template-engine-with-node-js-and-expressjs" class="btn btn-lg btn-secondary">Read More At Medium</a>
</p>
</main>
<%- include('../template/footer')-%>
</div>
</body>
</html>
```
EJS uses <%- include(‘’)-%> tag to include HTML from other files, in our app, we have the HTML templates at /views/template folder.

## Render Links
```
<%- include('../template/head')-%>
<body class="text-center">
<div class="cover-container d-flex w-100 h-100 p-3 mx-auto flex-column">
<%- include('../template/nav')-%>
<main role="main" class="inner cover">
<h1 class="cover-heading">Example with Links</h1>
<ul class="list-group">
<% links.forEach(function(entry) {%>
<a href="<%= entry.url%>" class="list-group-item text-dark"><%=entry.name%></a>
<%});%>
</ul>
</main>
<%- include('../template/footer')-%>
</div>
</body>
<script>
//Set active nav link
window.onload = function() {
document.getElementById('links').classList.add('active');
};
</script>
</html>
```
This time at res.render function after the name of the file we want to render we pass a JSON object.
```
res.render('pages/links',{
links:items
});
```
This JSON object will pass to the view pages/links.ejs. At this point, we use foreach function to iterate the links array and use “<%=” tag to output the properties url and name.
```
<% links.forEach(function(entry) {%>
<a href="<%= entry.url%>" class="list-group-item text-dark"><%=entry.name%></a>
<%});%>
```
## Render List
```
<%- include('../template/head')-%>
<body class="text-center">
<div class="cover-container d-flex w-100 h-100 p-3 mx-auto flex-column">
<%- include('../template/nav')-%>
<main role="main" class="inner cover">
<h1 class="cover-heading">List Example</h1>
<ul class="list-group">
<%list.forEach(function(entry) {%>
<li class="list-group-item text-dark"><%=entry%></li>
<%});%>
</ul>
</main>
<%- include('../template/footer')-%>
</div>
</body>
<script>
window.onload = function() {
document.getElementById('list').classList.add('active');
};
</script>
</html>
### Render Table
```
```
<%- include('../template/head')-%>
<body class="text-center">
<div class="cover-container d-flex w-100 h-100 p-3 mx-auto flex-column">
<%- include('../template/nav')-%>
<h1 class="cover-heading">Table Example</h1>
<div class="container bg-light text-dark">
<table class="table table-striped">
<thead>
<tr>
<th>Framework</th>
<th>URL</th>
</tr>
</thead>
<tbody>
<%table.forEach(function(entry) {%>
<tr>
<td><%=entry.name%></td>
<td><%=entry.url%></td>
</tr>
<%});%>
</tbody>
</table>
</div>
<%- include('../template/footer')-%>
</div>
</body>
<script>
window.onload = function() {
document.getElementById('table').classList.add('active');
};
</script>
</html>
```

### Features

* Fast compilation and rendering

* Simple template tags: <% %>

* Custom delimiters

**Includes:**

1- Both server JS and browser support

2- Static caching of intermediate JavaScript

3- Static caching of templates

4- Complies with the Express view system