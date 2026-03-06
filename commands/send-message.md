# Send a Message

Help the user send a message to an associate via SMS, email, or push notification.

## Steps

1. **Who is this for?** Ask for the associate's name. Use `list_associates` to find them and confirm.

2. **Check templates** — Call `list_messages_templates` to show available message templates. Ask if they want to use a template or write a custom message.

3. **Message content** — If using a template, fill in any template variables. If custom:
   - Ask for the message body
   - Optionally ask for a subject line

4. **Delivery channel** — Ask how they want to send it:
   - SMS (text message)
   - EMAIL
   - PUSH (push notification)
   Check that the associate has the relevant contact info (phone for SMS, email for EMAIL).

5. **Review and confirm** — Show the message preview before sending. Ask the user to confirm.

6. **Send** — Call `create_message` with the collected data. Show confirmation.

Keep it simple. Most users just want to send a quick message.
