---
title: "Contact"
layout: "page/contact"
---

Drop me a message if you want to say Hi :)

<form name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field" action="/contact/thank-you/" style="max-width: 600px; margin: 20px 0;">
  <input type="hidden" name="form-name" value="contact" />
  <p style="display: none;">
    <label>Don't fill this out if you're human: <input name="bot-field" /></label>
  </p>
  
  <div style="margin-bottom: 15px;">
    <label for="name" style="display: block; margin-bottom: 5px; font-weight: bold;">Name:</label>
    <input type="text" id="name" name="name" required minlength="2" maxlength="50" style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="email" style="display: block; margin-bottom: 5px; font-weight: bold;">Email:</label>
    <input type="email" id="email" name="email" required pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$" style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
    <small style="color: #666; font-size: 12px;">Please enter a valid email address</small>
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="subject" style="display: block; margin-bottom: 5px; font-weight: bold;">Subject:</label>
    <input type="text" id="subject" name="subject" required minlength="3" maxlength="100" style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="message" style="display: block; margin-bottom: 5px; font-weight: bold;">Message:</label>
    <textarea id="message" name="message" required minlength="10" maxlength="1000" rows="6" style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box; resize: vertical;"></textarea>
    <small style="color: #666; font-size: 12px;">Minimum 10 characters, maximum 1000 characters</small>
  </div>
  
  <button type="submit" style="background: #007cba; color: white; border: none; padding: 10px 20px; border-radius: 4px; cursor: pointer; font-size: 16px;">Send Message</button>
</form>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const form = document.querySelector('form[name="contact"]');
  const emailField = document.getElementById('email');
  
  // Enhanced email validation
  function validateEmail(email) {
    const re = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
    return re.test(email);
  }
  
  emailField.addEventListener('blur', function() {
    if (this.value && !validateEmail(this.value)) {
      this.style.borderColor = '#dc3545';
      this.setCustomValidity('Please enter a valid email address');
    } else {
      this.style.borderColor = '#ddd';
      this.setCustomValidity('');
    }
  });
  
  form.addEventListener('submit', function(e) {
    const email = emailField.value;
    if (!validateEmail(email)) {
      e.preventDefault();
      emailField.style.borderColor = '#dc3545';
      emailField.setCustomValidity('Please enter a valid email address');
      emailField.reportValidity();
      return false;
    }
  });
});
</script>

