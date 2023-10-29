### script
```js
  const root = document.getElementById("root");
      const first_h1_element = React.createElement( "h1",{ className: "parent-title" },"I am parent.");
      const second_h1_element = React.createElement( "h1",{ className: "parent-title" },"I am parent two.");
      const first_p_element = React.createElement("p", {}, "Barir Korta");
      const second_p_element = React.createElement("p",{},"Barir Second Korta");

      const element = React.createElement("div", { className: "wapper" }, [
        React.createElement("div", { className: "parent" }, [first_h1_element, "",first_p_element,]),
        React.createElement("div", { className: "parent-two" }, [second_h1_element,"", second_p_element,]),
        ]
    );

      ReactDOM.render(element, root);
```

### generated html
```html
<div id="root">
  <div class="wapper">
    <div class="parent">
      <h1 class="parent-title">I am parent.</h1>
      <p>Barir Korta</p>
    </div>
    <div class="parent-two">
      <h1 class="parent-title">I am parent two.</h1>
      <p>Barir Second Korta</p>
   </div>
 </div>
</div>
```



### Q1. What is the difference between a library and a framework?

<details><summary><b>Answer</b></summary>
<p>
library is some function to solve single problem but framework solve more than one problem and it's collection of library.
</p>
</details>

### Q2. What is CDN? Why do we use it?

<details><summary><b>Answer</b></summary>
<p>
  
`Content Delivery Network` (CDN) also known as `content distribution network`.It is a network of connected servers that speeds up webpage loading for data-heavy applications, reduce bandwidth costs and improve website security.
</p>
</details>

### Q3. What is cross-origin in the script tag?

<details><summary><b>Answer</b></summary>
<p>
The crossorigin attribute in the <script> tag is used to enable Cross-Origin Resource Sharing (CORS) for the script. CORS allow resource a web page to requeste other origin or domain.

When a web page loads a script from a different domain, it is considered a `cross-origin` request. By default, browsers restrict these types of requests for security reasons. The crossorigin attribute tells the browser to allow the different domain or origin (cross-origin) request.

It can have two values:

`anonymous`: A simple cross-origin request is made. No credentials are sent.
<br />
`use-credentials`: A cross-origin request is made with credentials. Cookies, HTTP authentication, etc. are sent.
</p>
</details>

### Q4. What is the difference between React and ReactDOM?

<details><summary><b>Answer</b></summary>
<p>
  
`React` is the view library which is used to build the components and `ReactDOM` is used to render React components into the DOM (Document Object Model). `ReactDOM` is like bridge of React to DOM.
</p>
</details>

### Q5. Difference between react.development.js and react.production.js files via CDN?

<details><summary><b>Answer</b></summary>
<p>
The React library provides two versions of its JavaScript files:

- `react.development.js`
- `react.production.js`
  
`react.development.js`:

- It is larger in size but easier to debug.
- provides more detailed error messages

`react.production.js`:

- It is optimized for performance and has a smaller file size
- has generic error messages for security
</p>
</details>

