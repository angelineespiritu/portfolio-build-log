# Refining the case-study reading experience

The page felt uneven, with too much open space on the right. I wanted the reading column and the table of contents to read as one composition.

I asked Cursor to measure the layout before I moved the body. The body was already centered. The TOC was anchored to a wider rail and sat far from the reading column. I brought it closer while preserving equal body margins. With that change, the navigation and the writing sat together.

I also reconsidered when the TOC should collapse, so it remained available on ordinary desktop widths. On narrower screens it becomes the compact “On this page” control, once the margin can no longer hold it.

Standard figures now share the prose column. Compact images stay small and can still be enlarged. Their captions are centered and use the full width of the reading column.

The introduction follows the same column. The outcomes stay side by side while they remain easy to read, then stack. I rejected an arrangement that lined the labels up by pulling Role and Timeline away from their values.

I wanted the layout to stay balanced without JavaScript repeatedly measuring and repositioning it. I used CSS to express the relationship between the reading column and the TOC, while keeping JavaScript for navigation and interaction. I removed the superseded measurements and rules, then checked the homepage and an article to make sure the shared navigation styles still worked as expected.

The prototype under “Explore the workflow” was missing because the renderer discarded embed blocks. Supporting those blocks, and using the published app URL, brought it back.

Earlier layout. The figure extends past the paragraphs, and the TOC sits far from the reading column.

![Earlier layout. The figure extends past the paragraphs, and the TOC sits far from the column.](./assets/before-body-overview.jpg)

Current layout, same section. The figure lines up with the paragraphs, and the surrounding prose stays in view.

![Current layout. The Overview figure lines up with the paragraphs.](./assets/after-body-overview.png)

Current layout, on a narrower desktop. The TOC is still beside the column.

![Current layout. The TOC remains beside the column on a narrower desktop.](./assets/current-workflow-1280.png)

Current layout, on a narrow screen. The figure and its caption stay in the column, and the TOC is the compact control.

![Current layout. On a narrow screen the caption stays centered in the column.](./assets/current-overview-figure-390.png)

Earlier caption. The line was only as wide as the small image, so it stacked.

![Earlier layout. The caption is only as wide as the compact image.](./assets/intermediate-compact-caption.png)

Current caption. The image stays small, and the caption is centered across the reading column.

![Current layout. The compact image stays small, and the caption uses the column.](./assets/after-compact-caption-1024.png)

Cursor checked the rendered page at desktop, tablet, and mobile widths. The spacing I had approved held, and the page did not scroll sideways. In my own browser I opened, closed, and used the table of contents, enlarged a compact image, closed it with Escape, and scrolled.

This pass reinforced the value of investigating a visual imbalance before changing positions: the body was centered, but its relationship with the navigation needed work. Typography is next, followed by another review of wrapping, spacing, and layout.
