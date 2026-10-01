--Readme document for Ronald Wen, ronaldwen10@gmail.com--

A reminder on academic integrity, as described in the syllabus.

In general, the course staff expects that you will look at code and examples from many online resources as part of the assignments, particularly to resolve syntax and understand frameworks. We expect that you'll use other libraries you find, and will even require it in some assignments. These practices are often critical to the work of developers today. The best developers are adept at interpreting the examples they see, customizing them to their specific situation, and citing their sources so they can find them later. We expect you to do the same.

While learning from examples is encouraged, attempting to pass an existing project or example from the web as your own is not allowed. If you ever have a question about what is or is not appropriate, feel free to ask the course staff!

Talking to classmates about class material, assignment requirements, etc. is a great way to verify ideas and get feedback. But this distinctly does *not* permit attempting to pass off someone else's code as your own. Talking over ideas and approaches is allowed, but the work that you produce and submit must be your own.

1. How many assignment points do you believe you completed (replace the *'s with your numbers)?

10/10
- 1/1 Readme
- 2/2 Basic HTML content
- 1/1 Basic CSS styling
- 1/1 Advanced feature
- 2/2 Responsive layout
- 1/1 Passes validation checks
- 2/2 Embraces spirit of the assignment

2. What (a) basic features, (b) CSS features, and (c) advanced features did you include in your portfolio?

(a) Basic features
- Images with descriptive alt text: portrait photo, project logos, and a Boring Notch product screenshot inside a figure with a caption.
- Headings and paragraph text in a logical order (one h1 per page, h2 for sections, h3 for sub-sections).
- Links to external pages: GitHub, LinkedIn, the Framelight website, and each merged pull request.
- Multiple pages (index.html, projects.html, contact.html) with a shared navigation bar. The current page is marked with aria-current and highlighted.
- Semantic HTML: header, nav, main, section, article, aside, figure/figcaption, dl, footer.
- Custom icons from Bootstrap Icons (email, GitHub, LinkedIn, location, external link, merged check mark).

(b) CSS features
- Padding and margins tuned for readability: a consistent section rhythm, text columns capped at ~38rem, and tighter spacing on phones.
- A custom warm color palette defined once as CSS variables (paper background, charcoal text, rust accent), all combinations checked for WCAG AA contrast.
- Bootstrap helpers: grid, rounded-circle portrait, img-fluid, table and table-responsive, form-control/form-select.
- Google Fonts: Playfair Display for headings and Inter for body text, with Georgia/Times and Helvetica/Arial fallbacks.

(c) Advanced features
- Complex layout: sticky navigation bar that collapses into a menu button on small screens, plus a sticky sidebar table of contents on the projects page that moves above the content on tablets and phones.
- Accessible data table of merged open-source contributions, with a caption, column headers (scope="col") and row headers (scope="row") so screen readers announce each cell's context.
- Contact form using HTML forms: labeled inputs, email type, required fields, a select menu, and autocomplete hints. It submits via mailto since the site is static.
- Accessibility extras: a "Skip to main content" link, visible keyboard focus outlines, and reduced-motion support that turns off hover animations for users who ask for less motion.

Responsiveness: on desktop the home page shows the hero text beside the photo and three project cards in a row; on tablets the cards go to two columns; on phones the photo moves above the text, everything stacks to one column, heading sizes shrink, and the navigation collapses into a menu button.

3. Did you ignore any of the warnings or errors presented by the accessibility checker? If so, why does this not seem like an accessibility concern? If it's useful, you can consolidate your thoughts on multiple warnings/errors if the rationale is similar.

There were no errors and no contrast errors in WAVE on any page, and no HTML or CSS errors. I reviewed the remaining alerts/warnings and left them:
- "Redundant link" (WAVE, all pages): the "Ronald Wen" brand and the "Home" nav item both go to index.html, and on the contact page the footer repeats the GitHub/LinkedIn links. Linking the brand to home is a convention users expect, and the footer links are a consistent landmark across pages, so the repetition helps navigation rather than hurting it.
- "Long alternative text" (WAVE, projects page): the Boring Notch screenshot's alt text is long on purpose because it describes several parts of the interface (album art, controls, visualizer) that a screen reader user would otherwise miss.
- CSS validator warnings: validating by page URL also checks the Bootstrap stylesheet loaded from the CDN, which uses vendor-prefixed properties and CSS variables the validator flags as warnings. These are in third-party code, not my stylesheet, and they are not errors.

4. How long, in hours, did it take you to complete this assignment?

2 hours

5. What online resources did you consult when completing this assignment? (list specific URLs, describe queries to Generative AI, or use of AI-based code completion)

- https://getbootstrap.com/docs/5.3/ (grid, navbar, tables, forms)
- https://icons.getbootstrap.com/ (icons)
- https://fonts.google.com/ (Playfair Display, Inter)
- https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table (accessible table markup)
- https://webaim.org/techniques/skipnav/ (skip link)
- https://validator.w3.org/ and https://jigsaw.w3.org/css-validator/ (validation)
- https://wave.webaim.org/ (accessibility checking)
- Generative AI (Claude, via Claude Code) was used to help convert my existing personal portfolio content into plain HTML/CSS pages, write the stylesheet, and run the validation checks. I reviewed and edited the output.

6. What classmates or other individuals did you consult as part of this assignment? What did you discuss?

None.

7. Is there anything special we need to know in order to run your code?

No. Open index.html in a browser. Bootstrap, Bootstrap Icons, and Google Fonts load from CDNs, so an internet connection is needed for full styling. All images use relative paths.
The written content (project descriptions, bio) is adapted from my personal portfolio site, but this HTML/CSS version was built from the course starter code for this assignment.
