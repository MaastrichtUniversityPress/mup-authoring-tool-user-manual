# MUP Authoring Tool - Frequently Asked Questions


Have a question about writing or publishing your book? Start here!

These answers cover the current Windows desktop app, **MUP Authoring**. Inside the app, the heading is **MUP Authoring Tool**.

---

## Table of Contents

1. [Getting Started and Saving](#getting-started-and-saving)
2. [Writing and Formatting](#writing-and-formatting)
3. [Images and References](#images-and-references)
4. [Publishing and Troubleshooting](#publishing-and-troubleshooting)
5. [Versions and Sharing](#versions-and-sharing)
6. [Getting Help](#getting-help)

---

## Getting Started and Saving

### Q: Do I need a GitHub account before writing?

**A:** You can create and edit a local draft without signing in. Connect GitHub when you want to load an existing GitHub book or publish a version. Publishing also requires access to the organisation configured for your app.

### Q: Can I write without an internet connection?

**A:** Yes. You can work on your saved local draft in the desktop app. You need an internet connection to sign in to GitHub, load a GitHub book or version, or publish. Local edits are uploaded only when you publish.

### Q: Why does GitHub sign-in show a code?

**A:** The app uses device login to connect your GitHub account. On **"Connect GitHub"**, note the code and click **"Open GitHub device login"**. Sign in on GitHub, enter the code, and approve the requested access. Return to the app and wait for **"Signed in as"** followed by your name. If the code expires, start sign-in again.

### Q: Why do I need to sign in again after restarting?

**A:** Closing the desktop app ends its GitHub session. Sign in again to publish or load GitHub books. Your saved local draft is separate from the login session and remains available for editing.

### Q: Where is the Save button?

**A:** Your work is saved automatically on your computer. The desktop app uses its own local data folder; the browser version uses that browser's local storage. These are separate copies. You do not need a Save button. Local saving does not upload your latest edits to GitHub; that happens when you publish.

### Q: Can I have multiple books?

**A:** You can work with different GitHub books, but the app keeps only one current book locally. Confirming **"Replace draft"** after **New Book**, opening a GitHub book, and **Use for editing** replace that local copy. Preserve unpublished work before switching. Opening the same book from GitHub again also replaces your local edits.

### Q: What should I choose in Replace current draft?

**A:** Choose **"Keep current draft"** to cancel creating a new book, then click **"Resume Book"** to continue your draft. Choose **"Replace draft"** only after preserving any unpublished work you need. This confirmation applies to **New Book**; opening a GitHub book or using **Use for editing** also replaces the draft and is not protected by this confirmation.

### Q: Is Download .md a complete backup?

**A:** No. It downloads only the open section's generated Markdown. It does not include all chapters, image files, or all book settings. Before switching books, publish a version when appropriate and confirm its build succeeded. If you cannot publish, copy each section's writing-area text into separate files and keep the original images, bibliography details, book title, and chapter order. You can also download each section's Markdown. See [Preserve Work Before Switching Books or Versions](USER_MANUAL.md#preserve-work-before-switching-books-or-versions).

### Q: Can I import a whole book from a file?

**A:** The current interface does not have a full-book file import or one-click restore button. You can open an approved TeachBooks project through **GitHub Books → Edit**, or paste saved writing-area text into sections and add the original images using **Add image**. Recreate references separately. If you paste generated Markdown, its heading and formatting marks may need adjustment; check the Live preview, image paths, and citations.

### Q: Does Close Book delete my book?

**A:** No. It returns you to the home page and keeps the current local draft. Click **"Resume Book"** to reopen it. It does not delete your GitHub repository or published versions, and it does not publish your latest edits.

### Q: How do I continue writing after closing or restarting the app?

**A:** The desktop app opens the home page on startup. Click **"Resume Book"** to continue the saved local draft, including unpublished edits. The same button is available after **Close Book**. Loading the book from GitHub instead replaces that draft with the saved GitHub content.

---

## Writing and Formatting

### Q: Why does a new book already have an Introduction and a chapter?

**A:** These are created for you so you can start writing immediately. Replace the sample introduction, open the first chapter, give it a title, and add content.

### Q: Where is the Markdown panel?

**A:** Turn on **"Markdown preview"** above the editor. You write in **"Start with your ideas"**; the Markdown panel shows generated output.

### Q: Why did my short sentence become a heading?

**A:** The first ordinary text line becomes the main heading. Later lines of up to 10 words and 80 characters can become section headings if they do not end with a period or comma. Start a line with a backslash if it should stay a paragraph:

```text
\This stays ordinary text
```

The backslash will not appear in the output.

### Q: Why did the first item in my list or quote become a heading?

**A:** The converter treats the first ordinary text line as the page heading, even if it begins with a list or quote marker. Start the section with a heading, then add your list or quotation below it. Check the Live preview before publishing.

### Q: What if I make a mistake in my formatting?

**A:** Check the **Live preview**. Edit the formatting marks in the writing area and review the result. For links inserted with **Link**, remember to replace the example address.

### Q: Can I reorganize my chapters?

**A:** Yes! Drag chapter cards before or after each other on the book page. The Introduction and Bibliography stay fixed.

### Q: Why can't I remove the last chapter?

**A:** A book must keep at least one chapter. The Introduction is separate and does not count as that chapter. Rename and rewrite the remaining chapter if you need different content.

### Q: What happens if I delete a chapter?

**A:** After you confirm **"Delete chapter"**, it is removed from the current book. There is no chapter restore button. Earlier published snapshots are separate, but loading one replaces your local working copy.

### Q: Is Load Example safe to try in a chapter I am writing?

**A:** It replaces the open section's text immediately and saves that change. Use a spare chapter or copy your text first. **Clear chapter** also changes the content immediately.

### Q: Can I use special characters or emojis?

**A:** Yes! Check them in the Live preview and published book. For version names, use simple, distinctive letters and numbers so the saved name is easy to recognize.

### Q: How long can my book be?

**A:** The app does not show a fixed chapter or word limit. Local storage, image sizes, and publishing resources still have practical limits. Keep images reasonably sized and preserve copies of important work.

---

## Images and References

### Q: Why doesn't typing an image filename make the image appear?

**A:** The app needs the actual image file, not just its name. Place the cursor in your text and use **"＋ Add image"** to choose the file. The app saves it with the book and inserts the image text.

### Q: What is alt text?

**A:** A description of what an image shows, such as "Diagram showing the water cycle." Enter it before adding the image. If left blank, the app uses the filename without its extension, which may not be a useful description.

### Q: What should I do if an image is missing?

**A:** Check the image path in your text. The app can try to recover saved images from a connected GitHub book. If the image is still missing, add the original file again and replace or remove the old broken image text. Run **Readiness Check** again.

### Q: Do I need images or a bibliography to publish?

**A:** No. A text-only book can be published. If you use citations, their references must exist in the bibliography.

### Q: Why is Insert Citation unavailable?

**A:** Add a bibliography and at least one reference first. Then open a regular chapter, choose a source under **"Cite a reference"**, and click **"Insert Citation"**.

### Q: What is the difference between a citation and Chapter References?

**A:** A citation is inserted at your cursor in the text. Chapter References is the list of selected sources shown at the end of the chapter when **"Show in chapter"** is enabled. Inserting a citation automatically selects its source and enables that list.

### Q: What happens when I remove a bibliography reference?

**A:** The source is removed from the bibliography and chapter selections. Citation text already written in your chapters remains. Update or remove those citations, then run **Readiness Check**.

---

## Publishing and Troubleshooting

### Q: What does Readiness Check actually check?

**A:** It checks the book title, chapter content and duplicate titles, saved images, references, and whether TeachBooks files can be generated. It does not check spelling, guarantee that links work, or test GitHub publishing permissions.

### Q: What is the difference between a blocker and a warning?

**A:** A blocker must be fixed before publishing. A warning asks you to review something, such as missing image alt text, but does not stop publication.

### Q: Why does my button say Publish Book Preview instead of Publish?

**A:** The button starts as **"Publish"** and can change to **"Publish Book Preview"** after a publishing attempt. It is the same publishing action.

### Q: How do I choose a version name?

**A:** Use a short name such as **"first draft"**, **"second draft"**, or **"2026 edition"**, with a maximum of 64 characters. Check **"Saved as"** before confirming: spaces become hyphens, letters become lowercase, and unsupported characters are removed. **"First Draft"** becomes **"version/first-draft"**. The names `main` and `master` are not allowed. Names also cannot contain consecutive periods or end in a period or `.lock`.

### Q: Why does the app say my version already exists?

**A:** Each saved version name must be unique within the book. Different names can become the same saved name: **"First Draft"** and **"first-draft"** both become **"version/first-draft"**. Choose a new name and check **"Saved as"**.

### Q: Where does the app create my book's GitHub repository?

**A:** In the organisation configured for your app, rather than in your personal GitHub account. Your account must be allowed to create repositories there. An existing GitHub-connected book continues to use its linked repository.

### Q: What should I choose in Create Repository?

**A:** **Public** makes the book's repository public. **Private** restricts access to its files on GitHub. This setting does not itself make the published website private. Confirm the intended access with your administrator if the book should have restricted readership.

### Q: What does Repository Exists mean?

**A:** A repository matching the name generated from your book title already exists. Choose **Cancel** and change the book title for a separate book. Choose **Overwrite** only when you intend to update the files in the repository shown. Overwrite does not allow you to reuse an existing version name.

### Q: GitHub is not connected. What should I do?

**A:** Click **"Sign in with GitHub"**, complete device login, and check for **"Signed in as"** before publishing. If the app says the session has expired, sign in again. If it reports a missing GitHub App or organisation configuration, ask your administrator to check the setup.

### Q: Why does the app say this book is unavailable or access is denied?

**A:** Signing in does not grant access to every repository. Ask your administrator to check that the GitHub App is installed for the configured organisation, the repository is selected for the App, and your account has the required access. Signing in again alone may not resolve an installation or permissions problem.

### Q: Why isn't my book in GitHub Books?

**A:** The list shows approved repositories in the configured organisation that your account can access and that the app recognises as TeachBooks projects. It does not list all personal repositories. Check the connected account and click **Refresh**. If the book is still missing, ask your administrator to check your access, the GitHub App's selected repositories, and the book's TeachBooks structure.

### Q: Why couldn't the app create my repository?

**A:** The name may be unavailable, or organisation policy may prevent repository creation or the selected visibility. Check the error message. Ask your administrator to check your account's ability to create repositories and the GitHub App permissions. For a separate book whose repository name already exists, cancel publishing and choose a different book title.

### Q: Why could GitHub Pages not be enabled?

**A:** The app could not enable website hosting for that repository. Check the message under **"What to do next"**. Ask your administrator to check whether Pages is available and allowed for that repository and account before changing repository visibility.

### Q: How long does publishing take?

**A:** It depends on the book and GitHub's build queue. Keep the app open and watch the progress. If it reports that the build is taking longer than expected, open the repository's **Actions** tab to see whether it is still running.

### Q: My files uploaded, but the build failed. Is the book published?

**A:** The new version is not confirmed ready. Open the GitHub Actions run named in the error details and check the failed step. Follow the issue panel's instructions or ask your administrator for help. Check whether the version name was already created before retrying.

### Q: Can I retry with the same version name after an error?

**A:** Only if that version was not already created. A failure can happen after the version has been saved to GitHub. Check **Published Versions** and the repository's **Actions** tab. If the name already exists, use a new version name after resolving the issue.

### Q: Why does a version appear in history but its link does not work?

**A:** The version's files can be saved before the website finishes building. The history entry and **Latest** badge do not prove that the build succeeded. Check GitHub Actions, wait for completion, and reopen the link.

### Q: What information should I send when reporting a publishing problem?

**A:** Include the book and version name, the action you took, the messages under **"What happened"** and **"What to do next"**, and relevant **"Technical details"**. If a build failed, include the GitHub Actions run link and failed step. Do not include passwords or GitHub login codes.

[image] Publishing issue panel: outline What happened, What to do next, and the Technical details control.

---

## Versions and Sharing

### Q: Can I edit my book after publishing?

**A:** Yes! Edit your chapters, then publish with a new version name. The previous published snapshot remains available through its own version link.

### Q: Can I update an existing named version?

**A:** The current app blocks reuse of existing version names. Publish a new name, even for a small correction.

### Q: What does Use for editing do?

**A:** It loads the selected published version as your current working copy. It replaces local unpublished content rather than merging it. Preserve your current work before switching.

### Q: Where did my Preview URL go?

**A:** The success panel is temporary and also closes when you use its Open link. Find the book's **Published Versions** section, click **Refresh**, and use **Copy link** beside the version you want.

### Q: Which link should I share?

**A:** Use **Copy URL** after a successful publication or **Copy link** beside the specific version in Published Versions. Open it yourself first to confirm the intended book and version.

### Q: Do I have to click Done before publishing?

**A:** No. **Done** is not available yet. Publish using **Publish**, wait for a successful build, then open and check the version link before sharing it.

### Q: Why does Done say Coming in a future update?

**A:** This is the current behaviour. The button opens **"Coming in a future update"**; click **"Close"** to dismiss it. It does not send an email, publish a version, or mark your book complete. When the book is ready for review, share its checked published version link with your editor through your usual communication channel.

---

## Getting Help

### Q: Who should I contact for help?

**A:** Start with the **"?"** guided tour, the [User Manual](USER_MANUAL.md), or the [First Publishing Workflow](FIRST_PUBLISHING_WORKFLOW.md). For technical problems, contact [lucian.uritu@maastrichtuniversity.nl](mailto:lucian.uritu@maastrichtuniversity.nl). Include the screen, action, and error message. Your organisation's administrator can help with GitHub access and setup.

---

**Happy Writing! 📚**

Remember: Preserve your work before switching books, and check the online version before sharing its link!
