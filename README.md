# PAUZ website — Render deployment

This is a static website that displays the supplied PAUZ webpage export without changing its artwork, wording, colours, or layout.

## Files

- `index.html` — website entry point
- `assets/pauz-website.png` — supplied PAUZ webpage export

## Deploy with GitHub + Render

1. Create a new GitHub repository, for example `pauz-website`.
2. Upload `index.html` and the `assets` folder (keep the folder structure unchanged).
3. Commit the files to the repository.
4. In Render, choose **New + → Static Site**.
5. Connect your GitHub repository.
6. Set **Build Command** to blank / none.
7. Set **Publish Directory** to `.`
8. Click **Create Static Site**. Render will provide a public URL.

## Responsive behaviour

The exported page image uses `width: 100%` and `height: auto`, so it scales proportionally to the browser width without cropping or distorting the design.

## Important limitation

Because the supplied source is one flattened image export, its text, illustrations, buttons, and sections are not separate editable or interactive webpage elements. The page preserves the supplied visual exactly. To make the email form, navigation, and buttons functional, or to make mobile layouts rearrange into a dedicated mobile design, the original Figma layers/assets or a rebuilt HTML version will be needed.
