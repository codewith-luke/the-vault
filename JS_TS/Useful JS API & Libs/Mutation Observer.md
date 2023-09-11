https://developer.mozilla.org/en-US/docs/Web/API/MutationObserver

By making the content editable this will trigger DOM mutations. Creating our observer and the target node we are then able to watch over these changes.

```html
<ol contenteditable>
  <li>Press enter</li>
</ol>
```

```js
const targetNode = document.querySelector('ol');

const config = {
  attributes: true, 
  childList: true, 
  characterData: true
};
  
const callback = mutations => {  
  mutations.forEach(mutation => {
    if (mutation.type === 'childList') {
      debugger;
      const listValues = Array.from(targetNode.children)
          .map(node => node.innerHTML)
          .filter(html => html !== '<br>');
      console.log(listValues);
    }
  });
}

const observer = new MutationObserver(callback);

observer.observe(targetNode, config);
```