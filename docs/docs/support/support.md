---
title: Support
permalink: /support/
layout: splash
tagline: "Create and Deploy a Backend Server"
description: "If you are a company that uses Djongo in your products, consider enrolling in a subscription plan. You get long term support."
excerpt: "If you are a company that uses Djongo in your products, consider enrolling in a subscription plan. You get long term support."

classes:
  - l-splash-full
  - feature-page
  - empty-banner
---

{% capture head %}
  {% include feature_page/support/tire.html %}
{% endcapture%}

{% capture content %}
  {% capture content%}
## Enterprise
If you are an enterprise that uses Djongo for commercial purposes, you need a license to use Djongo. Rights 
granted are: 

* Similar to a [MIT](https://opensource.org/licenses/MIT) style license.
* To use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software.

Get **phone, chat, and email support**. Send us a message for more information.
::
{% include form.html form=site.data.support.forms.enterprise %}  
  {% endcapture %}
  
{% include feature_page/flex.html 
    content=content %}
::

  {% capture content%}  
## Discuss
[Djongo forum](https://groups.google.com/forum/#!forum/djongo) is where you can watch for:

* New release announcements.
* Suggest improvements.
* Ask questions.
* Discuss topics pertaining to Django and MongoDB.

Alternatively, send us a message and we will get back to you.
::
{% include form.html form=site.data.support.forms.discuss %}
  {% endcapture %}

{% include feature_page/flex.html 
    content=content %}

{% endcapture %}

{% include feature_page/features.html 
    content=content 
    head=head %}