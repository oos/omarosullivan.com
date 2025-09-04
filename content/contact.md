---
title: "Contact"
---

Drop me a message if you want to say Hi :)

<form name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field" style="max-width: 600px; margin: 20px 0;">
  <input type="hidden" name="form-name" value="contact" />
  <p style="display: none;">
    <label>Don't fill this out if you're human: <input name="bot-field" /></label>
  </p>
  
  <div style="margin-bottom: 15px;">
    <label for="name" style="display: block; margin-bottom: 5px; font-weight: bold;">Name:</label>
    <input type="text" id="name" name="name" required style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="email" style="display: block; margin-bottom: 5px; font-weight: bold;">Email:</label>
    <input type="email" id="email" name="email" required style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="subject" style="display: block; margin-bottom: 5px; font-weight: bold;">Subject:</label>
    <input type="text" id="subject" name="subject" required style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box;">
  </div>
  
  <div style="margin-bottom: 15px;">
    <label for="message" style="display: block; margin-bottom: 5px; font-weight: bold;">Message:</label>
    <textarea id="message" name="message" required rows="6" style="width: 100%; padding: 8px; border: 1px solid #ddd; border-radius: 4px; box-sizing: border-box; resize: vertical;"></textarea>
  </div>
  
  <button type="submit" style="background: #007cba; color: white; border: none; padding: 10px 20px; border-radius: 4px; cursor: pointer; font-size: 16px;">Send Message</button>
</form>

