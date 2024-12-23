# Playwright Automation test

[Rference](https://playwright.dev/docs/intro)

## Important commands to be used :

1. npx playwright test

- Will run the test in all browsers.

2. npx playwright test to-picker.spec.js --project=chromium --headed

- It will run the test in chrome browser headed mean physically it will be visible like video

3.  npx playwright test to-picker.spec.js :171 --project=chromium --headed --debug

- This command will open the debig console and it is useful in debuggging and also we can record or write script while debugging from debugging console.

## Permision for camera to open camera for scanner

```Javascript
 // Launch a Chromium browser instance with camera permissions enabled
  const browser = await chromium.launch({
    headless: false, // Set to false if you want to visually confirm camera usage
  });

  // Create a new browser context with camera permissions
  const context = await browser.newContext({
    permissions: ["camera"], // Grant camera access
  });
```
