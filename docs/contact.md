---
layout: page
title: Contact
standfirst: I'd love to hear from you.
description: Get in touch with Agnès Déglon-Fischer.
permalink: /contact/
wide: true
redirect_from:
  - /contact-me/
---

{%- comment %}
  MORE THAN ONE DOOR, 2026-10-16. The page was correct and nearly empty: one
  button, then the footer at 730px, which reads as unfinished rather than
  spare. The email is still the main way in; the places Agnes already writes
  stand beside it, so a reader who does not want to send mail has somewhere
  to go instead of leaving.
{%- endcomment %}
<div class="split">
  <div class="split__main">
    <p>Whether you're an editor interested in my work, a reader with thoughts
      to share, or just someone who stumbled across my stories, feel free to
      reach out.</p>

    {% if site.contact_email and site.contact_email != "" %}
    <p style="margin-top:var(--sp-6)">
      <a class="btn btn--primary" href="mailto:{{ site.contact_email }}">Send me an email</a>
    </p>
    {% else %}
    <p><em>An address for messages is being set up. In the meantime, the chat
    assistant at the corner of the page can pass on a note.</em></p>
    {% endif %}
  </div>

  <div class="split__aside">
    <span class="label">Elsewhere</span>
    <p style="margin-top:var(--sp-4)">I also write in a few other places, and
      the letters are the surest way to hear from me.</p>
    <ul class="elsewhere">
      <li><a href="{{ '/newsletter/' | relative_url }}">The Path Is the Goal</a>
        — my letter from the writing desk, free, roughly every other week.</li>
      <li><a href="https://{{ site.substack }}" rel="noopener">Substack</a>
        — the letters, archived.</li>
      <li><a href="https://medium.com/@agnes.deglon" rel="noopener">Medium</a>
        — where several of these essays first appeared.</li>
    </ul>
  </div>
</div>
