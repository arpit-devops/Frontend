Here are short and simple notes on **jQuery**:

---

### **1. What is jQuery?**
- jQuery is a **fast, small, and easy-to-use JavaScript library**.
- It makes tasks like **HTML manipulation, event handling, animation, and Ajax** much easier.
- It works across all major browsers (cross-browser support).

---

### **2. Why Use jQuery?**
- Less code, more functionality.
- Simplifies DOM manipulation and event handling.
- Easy to use animations and effects.
- Makes Ajax calls simpler.

---

### **3. Adding jQuery to a Page**
```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
```

---

### **4. Basic Syntax**
```javascript
$(selector).action();
```
- `$` = jQuery
- `selector` = HTML element
- `action()` = what you want to do

---

### **5. Examples**
```javascript
// Hide a paragraph
$("p").hide();

// Change text of an element
$("#title").text("Welcome!");

// Click event
$("#btn").click(function() {
  alert("Button clicked!");
});
```

---

### **6. DOM Ready Function**
Ensures code runs after the page is fully loaded:
```javascript
$(document).ready(function() {
// Write your jQuery code here to ensure it runs after the entire document is fully loaded
// Example:
$("p").css("color", "blue");

});
```