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

Implemented this:

```ts
const uuid = () =>
 typeof crypto.randomUUID === 'function'
   ? crypto.randomUUID()
   : `${Date.now()}-${Math.random().toString(16).slice(2)}`;

const subdomain = 'airbnb-parent';
const modelId = 'gpt-5.4';
const foreignKey = 'chat-attachments/6a509b55b6aa57b9698f3791/294c06b2a14b6c81747b2744ce54472abcdc329478828d22ddf063cafe79c44f-personal-linkedin.png';

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
            text: 'What is in the image? please describe it to me',
          },
          {
            type: 'file',
            key: foreignKey,
            mediaType: 'image/png',
            filename: 'personal-linkedin.pdf',
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

console.log('Status:', response.status);

const raw = await response.text();
let answer = '';

for (const line of raw.split('\n')) {
  if (!line.startsWith('data: ') || line === 'data: [DONE]') continue;

  try {
    const event = JSON.parse(line.slice(6));
    if (event.type === 'text-delta') {
      answer += event.delta;
    }
  } catch {
    // Ignore non-JSON stream lines.
  }
}

console.log('Answer:', answer);
```

```ts
const uuid = () =>
 typeof crypto.randomUUID === 'function'
   ? crypto.randomUUID()
   : `${Date.now()}-${Math.random().toString(16).slice(2)}`;

const subdomain = 'xata-29d07fe6';
const modelId = 'gpt-5.4';
const foreignKey = 'chat-attachments/6a509b55b6aa57b9698f3791/294c06b2a14b6c81747b2744ce54472abcdc329478828d22ddf063cafe79c44f-personal-linkedin.png';

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
            text: 'What is in the image? please describe it to me',
          },
          {
            type: 'file',
            key: foreignKey,
            mediaType: 'image/png',
            filename: 'personal-linkedin.pdf',
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

console.log('Status:', response.status);

const raw = await response.text();
let answer = '';

for (const line of raw.split('\n')) {
  if (!line.startsWith('data: ') || line === 'data: [DONE]') continue;

  try {
    const event = JSON.parse(line.slice(6));
    if (event.type === 'text-delta') {
      answer += event.delta;
    }
  } catch {
    // Ignore non-JSON stream lines.
  }
}

console.log('Answer:', answer);
```