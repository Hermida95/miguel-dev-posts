# 💡 HTML Tip: The `autocomplete` Attribute

Did you know you can improve form usability and help browsers autofill fields just with pure HTML?

The `autocomplete` attribute in `<input>` lets browsers suggest previously entered information.  
But even better: you can **specify the exact data type** so the browser recognizes it automatically.

## ✅ Example
```html
<form>
  <label for="email">Email:</label>
  <input type="email" name="email" autocomplete="email" />

  <label for="phone">Phone:</label>
  <input type="tel" name="phone" autocomplete="tel" />

  <label for="postal">Postal Code:</label>
  <input type="text" name="postal-code" autocomplete="postal-code" />
</form>

✅ Common autocomplete values

name
email
username
new-password
address-line1
cc-number
postal-code
and many more...

🔐 Benefits
Enhances accessibility and user experience
Increases security for login and payment forms
Zero JavaScript needed