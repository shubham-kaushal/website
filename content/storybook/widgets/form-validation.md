---
title: Form validation
description: Examples of form validation using Numl
---

```html
<split/>
<nu-form>
  <nu-field>
    <nu-label for="email">Email</nu-label>
    <nu-input id="email"></nu-input>
    <nu-check for="email" assert="required" color="hue(1)">
      Email is required
    </nu-check>
    <nu-check for="email" assert="email" color="hue(1)">
      A valid email address is required
    </nu-check>
  </nu-field>
  <nu-field>
    <nu-label for="password">Password</nu-label>
    <nu-input id="password"></nu-input>
    <nu-check for="password" assert="required" color="hue(1)">
      Password is required
    </nu-check>
    <nu-check for="password" assert="minlength:8" color="hue(1)">
      Password should be at least 8 characters long
    </nu-check>
  </nu-field>
  <nu-btn action="submit">Submit</nu-btn>
</nu-form>
```
