Here are short notes on **JavaScript DOM (Document Object Model):**

---

### **1. What is the DOM?** 

The **DOM (Document Object Model)** is like a **map of your webpage**.  
It turns your HTML into a **tree-like structure** that JavaScript can read and change.

Using the DOM, JavaScript can:
- Find things on the page (like buttons or text),
- Change how things look (like colors or fonts),
- Or respond to user actions (like clicks).

---

### **Example**  
Let’s say your HTML has this element:  
```html
<p id="test">Hello!</p>
```

You can use JavaScript to get this element and do something with it:
```javascript
var testElement = document.getElementById("test");
testElement.textContent = "Hi there!";
```

Now the text on the page will change from **Hello!** to **Hi there!**.


---

### **2. Accessing Elements**
- Use JavaScript methods to select elements:
  - `document.getElementById("id")`
  - `document.getElementsByClassName("class")`
  - `document.getElementsByTagName("tag")`
  - `document.querySelector("selector")`
  - `document.querySelectorAll("selector")`

---

### **3. Modifying Elements**
- **Content**:  
  - `element.textContent = "new text"`  
  - `element.innerHTML = "<b>Bold</b>"`
- **Attributes**:  
  - `element.setAttribute("src", "image.png")`  
  - `element.getAttribute("href")`
- **Styles**:  
  - `element.style.color = "red"`

---

### **4. Creating & Removing Elements**
- **Create**:  
  - `let div = document.createElement("div")`
- **Append**:  
  - `parent.appendChild(div)`
- **Remove**:  
  - `parent.removeChild(child)`

---

### **5. Event Handling**
- Use `addEventListener()` to handle user interactions:
  ```javascript
  element.addEventListener("click", function() {
    alert("Clicked!");
  });
  ```

---

### **6. DOM Tree**
- The HTML page is treated as a hierarchical tree:
  - `document` → root of the DOM
  - Nodes: elements, text, comments
  - You can navigate with properties like `parentNode`, `childNodes`, `nextSibling`, etc.

---

Let me know if you want a visual diagram or examples for practice!