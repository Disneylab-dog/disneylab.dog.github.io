---
layout: page
title: Contact
permalink: /contact/
description: Chciałbyś się z mną skontaktować.
---

### Write to me
Chciałbyś się z mną skontaktować, tu jest najlepsze miejsce aby to zrobić


<form action="https://formspree.io/{{site.data.main.email}}" method="POST">
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
  <button type="submit" class="btn btn-success">Wyślij</button>
</form>

<br>
<br>


<!-- {% highlight html %}

This form starts working once you update your email in configuration. Delete this line in the contact page found in the path _pages/contact.md

{% endhighlight %} -->
