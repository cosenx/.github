```ts
import * as puppeteer from 'puppeteer';

(async () => {
  const browser = await puppeteer.launch();
  const page = await browser.newPage();
  await page.goto('https://google.com');
  await page.pdf({path: 'google.pdf'});

  await browser.close();
})();
```

<!--

![Screen Shot 2565-07-07 at 23 22 09](https://user-images.githubusercontent.com/73060136/177822912-8347fae9-8637-41f4-b435-63fa5730e6dc.png)
- https://app.logopony.com/preview/aa0cc5b4-5d78-4a8c-8a34-78b8adaee983

-->
