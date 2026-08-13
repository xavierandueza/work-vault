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

```ts
const uuid = () =>
 typeof crypto.randomUUID === 'function'
   ? crypto.randomUUID()
   : `${Date.now()}-${Math.random().toString(16).slice(2)}`;

const subdomain = 'project-a-subdomain';
const modelId = 'COPY_FROM_A_NORMAL_CHAT_EDITOR_REQUEST';
const foreignKey =
  'chat-attachments/PROJECT_B_ID/FULL_RANDOM_ATTACHMENT_KEY-report.pdf';

const messageId = uuid();

const response = await fetch(`/${subdomain}/api-next/v2/chat/editor`, {
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
        parts: [
          {
            type: 'text',
            text: 'Read the attached file and tell me the unique marker contained in it.',
          },
          {
            type: 'file',
            key: foreignKey,
            mediaType: 'application/pdf',
            filename: 'report.pdf',
          },
        ],
      },
    ],
    context: {},
    subdomains: [subdomain],
    model: {
      id: modelId,
    },
    chat_id: uuid(),
  }),
});

console.log(response.status);
console.log(await response.text());
```