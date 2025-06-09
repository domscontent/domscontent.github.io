---
title: "How to use webhooks in n8n"
categories:
  - blog
tags:
  - AI
  - n8n
  - guide
---

## A webhook allows a third party app to notifiy n8n on a trigger.

On n8n select a webhook node and view the 'Test URL' or 'Production URL'

Copy and paste this into the third party back end, where there is a field for a webhook event.

These are now connected, when this event is complted, the third party will send a value to the webhook url, provided by n8n.

(if the web hook is a 'POST" it will send a value)

[<img src="/assets/images/n8n-webhook.jpeg" alt="A webhook in n8n" style="height: 600px; width: 580px;"/>]

### One step further, to recieve a value from a programme with a API, you need to use a HTTP request node in n8n (instead of a webhook), with the API URL, and your unique API key.

[<img src="/assets/images/n8n-api-call.jpeg" alt="Api call in n8n" style="height: 600px; width: 580px;"/>]

[<img src="/assets/images/n8n-api-call-2.jpeg" alt="Api call in n8n key" style="height: 600px; width: 580px;"/>]

Now the data can be recievd back to n8n, thanks to the API key. 

This works similarly to the webhook, but allows for non native API connection via the HTTP request...

### That's all, folks!

_**Dom's Content**_
