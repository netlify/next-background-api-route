# Next.js Background API Routes (Beta)

This is a psuedo-code demo of a Next.js API route running as a Background Function on Netlify.

Find the code in [batch-process.js](pages/api/batch-process.js) which mocks generating invoices, creating PDFs and
sending emails in a synchronous queue.

## Enable Background Functions in your Next.js project

Add the following code to any API route in a Next.js project running on Netlify.

```javascript
export const config = {
  type: "experimental-background",
};
```

[Learn more on the Netlify docs.](https://docs.netlify.com/integrations/frameworks/next-js/advanced-api-routes/)
