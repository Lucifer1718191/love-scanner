# love-scanner
Love Verdict Scanner

A fun single-page website. Upload a photo and the scanner shows a verdict on whether your love story will happen or not, with a match score and four score bars (smile factor, swag level, heart setting, luck signal).

This is just for fun. It has nothing to do with real relationships.

How it works
Choose a photo, or drag and drop one onto the frame.
A short scanning animation plays, then the verdict appears: It's a yes (match score 50% or more) or It's a no (below 50%).
The result depends only on the photo. The same photo always gives the same result, no matter how many times you scan it. A different photo can give a different result.
"Scan again" replays the scan animation and shows the same result.
Privacy

Your photo never leaves your device. It is read in your browser and is not uploaded to any server.

Files
File	What it is
index.html	The whole website: page, styles and script in one file
README.md	This file
Run it locally

Download the files and double-click index.html. It opens in your browser. No install or build step is needed.

The page loads fonts from Google Fonts, so fonts need an internet connection. Without it the page still works with default fonts.

Deploy for free
GitHub Pages
Upload index.html and README.md to a public GitHub repository.
Go to Settings, then Pages.
Under Source choose Deploy from a branch, select main and / (root), then Save.
After about a minute the site is live at https://<your-username>.github.io/<repo-name>/.
Netlify
Sign in at netlify.com.
Click Add new site, then Import an existing project, then Deploy with GitHub.
Select this repository. Leave the build command empty and set the publish directory to .
Click Deploy. Your site is live at a *.netlify.app link.

Once both are connected to the same repository, every change you commit to GitHub updates both sites automatically.

Customise

Everything is in index.html:

Text: headings, button labels and verdict messages are plain text in the HTML and in the reveal() function.
Colors and fonts: change the values at the top of the <style> block (:root). A dark theme is included and follows the visitor's device setting.
Verdict threshold: in reveal(), change pct >= 50 to move the line between yes and no.
