# Page contract for docs.madeformeai.com (customer guides), 2026-09-28

Who reads this: a small-business owner or their staff whom Dustin (Quick IT Projects) has already set up. They got the link in an email. They are not shopping. Nobody arrives here from the web.

Every page:
- Frontmatter: `title` (short, imperative where it is a task: "Log in", "Put it on your phone"), `description` (one plain sentence).
- Opens with one or two sentences saying what you will have when you are done. No preamble, no pitch.
- Body is numbered steps. Each step is one action, starts with a verb, names the exact button or menu item in **bold**. Sub-details go under the step as a short line, not a paragraph.
- Use Mintlify `<Steps><Step title="...">...</Step></Steps>` for the step list. `<Note>` for a small aside, `<Warning>` only for something that loses data or money. `<Frame>` around an existing screenshot when the page already has one; never invent an image path.
- Ends with an `## If this fails` section: two to four bullets, each "symptom -> what to do", the last one always "Still stuck: email support@madeformeai.com with a screenshot and the time it happened."
- Second person ("you"), present tense, short sentences. No em dashes (use a comma or a period). No "simply", "just", "easily", "seamlessly", "powerful", "robust". No exclamation marks.
- Zero sales language. Delete every "Want one?", "Start on the homepage", "Sign up free", "real customers run theirs", "I build it for you", any pricing, any feature that is "coming soon", any comparison to other products.
- Facts only from the source files named in your task. If a source does not say it, write nothing about it. Never guess a menu label; if the label is unknown in the sources, describe the location ("the menu under your name, top right").
- Do not mention: server or box names, the city any server is in, the login product by name (say "the login page"), n8n, Retell, tenant names, other customers, Dustin's infrastructure, env vars, API routes, Discord invites.
- Keep pages short: 40 to 120 lines. Split rather than scroll.
- Links between pages are root-relative Mintlify links: `[Put it on your phone](/guides/2-put-it-on-your-phone)`.
