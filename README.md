# Email Builder

## Install

```shell
npm i @uon/email
```


## Usage

```typescript

import { EmailMessage } from '@uon/email';

const msg = new EmailMessage()
    .from('me@me.com')
    .to('example@example.com')
    .subject('Hello World!')
    .html('<h1>Hi!</h1>')
    .text('Hi!')
    .attachment({
        name: 'image.png',
        mime: 'image/png',
        data: img_buffer
    });

const msg_buffer = msg.render();


```