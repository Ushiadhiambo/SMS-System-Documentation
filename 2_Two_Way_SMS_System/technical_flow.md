# Technical Flow of Two-Way SMS

## Overview

SMS messages flow through an SMS gateway platform and do not go directly between the user and business system.

### Workflow

1. **SMS Gateway provision:**  
   Business rents shortcode or purchases long code via an SMS gateway (e.g., Africa's Talking, Twilio).

2. **Sending Messages:**  
   Business application sends messages via the gateway's **API**.  
   Gateway delivers the SMS to the user's phone.

3. **Receiving Replies:**  
   User replies to the shortcode or long code.  
   SMS gateway receives the replies.  
   Gateway forwards replies to the business app through a **Webhook** (callback URL).

4. **Processing Replies:**  
   Business system parses reply.  
   Automated/manual responses are generated and sent back via the gateway.

---

## Required Components

- **API Access:** To send and receive SMS messages programmatically.  
- **Webhook (Callback URL):** Listens for inbound SMS replies.

---

## SMS Gateway Providers with APIs and Webhooks

- [Africa's Talking API Documentation](https://africastalking.com/docs)  
- [Twilio Messaging API](https://twilio.com/docs/sms)  
- [Infobip API](https://dev.infobip.com/sms)

---
