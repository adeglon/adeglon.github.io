---
layout: page
title: Contact
standfirst: I'd love to hear from you.
description: Get in touch with Agnès Déglon-Fischer.
permalink: /contact/
redirect_from:
  - /contact-me/
---

Whether you're an editor interested in my work, a reader with thoughts to share,
or just someone who stumbled across my stories, feel free to reach out.

{% if site.contact_email and site.contact_email != "" %}
<p style="margin-top:var(--sp-6)">
  <a class="btn btn--primary" href="mailto:{{ site.contact_email }}">Send me an email</a>
</p>
{% else %}
<p><em>An address for messages is being set up. In the meantime, the chat
assistant at the corner of the page can pass on a note.</em></p>
{% endif %}
