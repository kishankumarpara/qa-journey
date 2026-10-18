# Bug report



|Field|Content|
|-|-|
|Bug ID|BUG\_02|
|Related test case|TC\_06|
|Title|Login is slower for performance\_glitch\_user than for standard\_user|
|Environment|Microsoft Edge Version 155.0.4283.45 , Windows, saucedemo.com, 10/18/2026|
|Metric|Largest Contentful Paint (LCP) on the Products page after login|
|Steps to reproduce|1. Open saucedemo.com and press F12 to open DevTools.<br />2. Open the Performance tab and start recording with the page reload option.<br />3. Log in as `standard\\\_user` / `secret\\\_sauce`.<br />4. Stop recording and note the LCP value.<br />5. Log out and repeat steps 2-4 with `performance\\\_glitch\\\_user` / `secret\\\_sauce`.<br />6. Repeat the whole test 3 times for each user.|
|Expected result|LCP under 2.5 seconds (Google's "good" guideline, used here as the benchmark since the site has no stated requirement). `standard\\\_user` measured 0.14s.|
|Actual result|`performance\\\_glitch\\\_user` LCP: 5.23s (run 1) and (runs 2 and 3, which you should fill in).|
|Severity|Medium (login works, but the delay is clearly noticeable)|
|Priority|Low (affects a test account, not a standard user)|



