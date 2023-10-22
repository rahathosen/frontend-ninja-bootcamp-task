### code
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

### output
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



## Q1. What is the difference between a library and a framework?

<details><summary><b>Answer</b></summary>
<p>
library is some function to solve single problem but framework solve more than one problem and it's collection of library.
</p>
</details>

## Q2. What is CDN? Why do we use it?

<details><summary><b>Answer</b></summary>
<p>

</p>
</details>

## Q3. What is cross-origin in the script tag?

<details><summary><b>Answer</b></summary>
<p>


</p>
</details>

## Q4. What is the difference between React and ReactDOM?

<details><summary><b>Answer</b></summary>
<p>

</p>
</details>

## Q5. Difference between react.development.js and react.production.js files via CDN?

<details><summary><b>Answer</b></summary>
<p>

</p>
</details>

