---
layout: default
title: Contact
---

<div id="contact">
  <h1 class="pageTitle">Contact Me</h1>
  <div class="contactContent">
  <p class="intro">If you have any questions, feel free to contact me.</p>
  <img class="me" src="{{ '/assets/img/me.jpg' | prepend: site.baseurl }}" alt="">

  </div>
  <form action="http://formspree.io/ang.moyhour@outlook.com" method="POST">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" class="full-width"><br>
    <label for="email">Email Address</label>
    <input type="email" id="email" name="_replyto" class="full-width"><br>
    <label for="message">Message</label>
    <textarea name="message" id="message" cols="30" rows="10" class="full-width"></textarea><br>
    <input type="submit" value="Send" class="button">
  </form>
</div>
