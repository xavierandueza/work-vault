```ts
const uuid = () =>
 typeof crypto.randomUUID === 'function'
   ? crypto.randomUUID()
   : `${Date.now()}-${Math.random().toString(16).slice(2)}`;

let messageId = uuid();
let question = 'How do I authenticate?';
let subdomain = 'subdomain';

let response = await fetch(`/${subdomain}/api-next/v2/owlbot/conversation`, {
  method: 'POST',
  credentials: 'include',
  headers: {
    'Content-Type': 'application/json',
  },
  body: JSON.stringify({
    messages: [
      {
        id: messageId,
        role: 'user',
        parts: [{ type: 'text', text: question }],
      },
    ],
    question,
    chat_id: uuid(),
    message_id: messageId,
  }),
});

console.log(response.status, await response.text());
```