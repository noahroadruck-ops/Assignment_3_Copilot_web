# Desktop Social Media Website

## Project Goal

Build a basic social media home page designed primarily for a computer screen. Use HTML for page structure, CSS for the visual layout, and a small amount of JavaScript for interactions. The first version can use sample content and does not need accounts, a server, or a database.

## Page Outline

```text
+---------------------------------------------------------------+
| Header: site name / search / profile                          |
+----------+----------------------------------------------------+
|          | Stories: circular icons for followed people        |
| Left     +----------------------------------------------------+
| icon     | Main feed: post, post, post                         |
| bar      |                                                    |
|          |                                      Messages tab  |
+----------+----------------------------------------------------+
```

### 1. Overall Page and Header
- Create a desktop-first page with a header, a fixed left navigation bar, and a central content area.
- Give the site a temporary name and a simple profile area.
- Keep the layout readable at common laptop and desktop widths.

### 2. Left Navigation Bar
- Stretch the navigation bar from the top to the bottom of the window.
- Include icon buttons for Home, Search, Explore, Notifications, and Profile.
- Make Home visibly selected.
- Add a text label or tooltip for each icon so its purpose is clear.

### 3. Followed-People Row
- Place a horizontal row near the top of the central area.
- Show a circular image or colored placeholder for each followed person, with a name underneath.
- Give the circles a consistent size and spacing.
- Use sample names and local placeholder imagery or CSS colors; do not depend on a live social media API.

### 4. Main Post Feed
- Display several sample posts in a vertically scrolling central column.
- Each post should show an author avatar and name, a timestamp, post text, and an optional image area.
- Separate posts clearly without making the feed too wide.
- Use realistic sample content that makes the layout easy to evaluate.

### 5. Post Actions
- Add Like, Comment, and Share buttons to each post.
- Make Like toggle between liked and unliked states, and update a visible like count.
- Make Comment reveal a small comment input or comment area.
- Share can show a simple confirmation message; it does not need to publish externally.

### 6. Messages Tab
- Add a compact Messages button fixed near the bottom-right corner of the window.
- Clicking it should open and close a small messages panel.
- The panel can show a few sample conversations and a close button.
- Ensure it does not cover important post controls when open.

### 7. Final Checks
- Check that the left bar stays in place while the feed scrolls.
- Check that stories remain near the top of the feed area.
- Try each navigation and post-action button, plus opening and closing Messages.
- Check the page at a typical desktop width and at a narrower window width; prevent horizontal overflow.
- Keep the HTML organized with semantic elements and give buttons accessible names.

## Prompt-Engineering Sequence

Use one prompt at a time, inspect the result, and then move to the next part. Keep each change limited to the requested section.

1. **Create the skeleton**

	> Create a semantic HTML skeleton for a desktop-first social media home page. Include a header, a full-height left navigation area, a central content area with a followed-people row and post feed, and a fixed Messages button in the bottom-right. Use placeholder content only. Do not add interactions yet. Keep the HTML readable and accessible.

2. **Style the layout**

	> Style the existing page with CSS for a desktop social media site. Keep the left navigation full-height, put the followed-people row above the central feed, constrain the feed width, and fix the Messages button near the bottom-right. Use consistent spacing and make the layout avoid horizontal overflow at narrower window widths. Do not change the existing HTML structure unless necessary.

3. **Build the followed-people row**

	> Complete the followed-people row using circular avatars or attractive local placeholders, with a name below each circle. Keep avatar dimensions consistent and make the row horizontally scrollable if it cannot fit. Do not add external services or dependencies.

4. **Build sample posts**

	> Add several sample posts to the central feed. Each post should include an author, avatar, timestamp, text, optional image placeholder, and Like, Comment, and Share controls. Match the page's existing visual style and keep each post easy to scan.

5. **Add post interactions**

	> Add simple JavaScript interactions to the existing post controls: Like toggles its state and count, Comment reveals a comment input or area, and Share shows a brief confirmation. Keep the implementation local to this page; no backend or external service is needed.

6. **Add the messages panel**

	> Make the fixed Messages button open and close a compact messages panel near the bottom-right of the page. Include a few sample conversations and a close control. Ensure the panel stays within the viewport and does not block the page unnecessarily.

7. **Review and test**

	> Review the existing page against this checklist: desktop layout, full-height left navigation, followed-person circles above the feed, readable sample posts, working Like/Comment/Share controls, working Messages open/close behavior, accessible button names, and no horizontal overflow. Make only fixes needed to satisfy the checklist, and summarize what you changed.

## Suggested Build Order

Start with the HTML skeleton, then establish the desktop layout before adding detailed styling. Add sample content next, implement interactions after the structure is stable, and finish by checking the page at multiple window widths.