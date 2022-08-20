---
layout: page
title: Kontakt
permalink: /kontakt/
description: Chciałbyś się z mną skontaktować.
---

### Write to me
Chciałbyś się z mną skontaktować, tu jest najlepsze miejsce aby to zrobić

<script src="https://www.google.com/recaptcha/api.js" async defer/>
<script>
  window.onload = function() { 
  var el = document.getElementById('g-recaptcha-response'); 
  if (el) { 
    el.setAttribute('required', 'required'); 
  } 
</script>
<style>
  #g-recaptcha-response {
    display: block !important;
    position: absolute;
    margin: -50px 0 0 0 !important;
    z-index: -999999;
    opacity: 0;
  }
</style>

<form action="https://formspree.io/f/{{site.data.main.formspree.form}}" method="POST">
  <div class="form-group">
    <label for="email">Adres email</label>
    <input type="email" name="email" class="form-control" placeholder="Wprowadź swój adres email">
  </div>
  <div class="form-group">
    <label for="message">Wiadomość</label>
    <textarea class="form-control" name="content" id="" rows="3" placeholder="Napisz do mnie:)"></textarea>
  </div>
  <input type="hidden" name="_next" value="{{site.url}}{{page.url}}">
  <input type="hidden" name="_subject" value="New Contact Form Submission">
  <input type="text" name="_gotcha" style="display:none">
  <div class="g-recaptcha" data-sitekey="{{site.data.main.formspree.recapatcha}}"></div>
  <br/>
  <button type="submit" class="btn btn-success">Wyślij</button>
</form>



<!-- {% highlight html %}

This form starts working once you update your email in configuration. Delete this line in the contact page found in the path _pages/contact.md

{% endhighlight %} -->
