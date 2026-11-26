# My Media — Website Starter

A responsive, dark-first video discovery website prototype built with plain HTML, CSS and JavaScript. It is designed to publish on GitHub Pages.

## Files

- `index.html` — website structure and page metadata
- `css/style.css` — layout, colors, responsive design and theme styles
- `js/videos.js` — sample video feed data
- `js/app.js` — search, category filters, likes, saves, follows, local video preview and modal interactions
- `assets/favicon.svg` — My Media browser icon

## Publish on GitHub Pages

1. Download and extract the ZIP file on your device.
2. Open your GitHub repository.
3. Choose **Add file → Upload files**.
4. Upload the contents of the extracted `My-Media-Website` folder. Make sure `index.html` is directly in the repository root, not inside an extra nested folder.
5. Commit the uploaded files to the `main` branch.
6. Open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Select branch `main` and folder `/ (root)`, then Save.
9. Wait for GitHub Pages to publish the site. The public URL will appear in the Pages settings.

## Video samples

The demo feed uses YouTube embedded players. You can replace the sample video IDs in `js/videos.js` with IDs of videos that you own or are allowed to embed. Some video owners disable embedding, and some videos may be unavailable in certain regions. In that case the player may show an error. See the [YouTube embed help](https://support.google.com/youtube/answer/171780) and [YouTube IFrame Player API documentation](https://developers.google.com/youtube/iframe_api_reference).

## Important: prototype limitations

This is a front-end website prototype. GitHub Pages is static hosting, so this package does **not** include:
- real user registration, login or password storage
- permanent video uploads or cloud storage
- a shared database for likes, comments, follows or profiles
- moderation, notifications, recommendation algorithms or admin dashboard

Likes, saved videos, follows and theme preference are stored in the visitor's browser using local storage. The upload control previews a selected video locally; it does not send it to the internet. Comments are a demonstration only.

To launch a real public video-sharing platform, connect a secure backend, database, authentication, video storage/transcoding and moderation system. Never put private API keys or passwords in frontend JavaScript.

## Customizing the sample feed

Open `js/videos.js`. Each entry contains:
- `youtubeId`: YouTube video ID
- `title`: video title
- `creator`, `handle`, `initial`: creator display information
- `category`: Creative, Nature, Technology or Animation
- `views`, `likes`, `description`: sample display data

Replace sample entries with content you have rights to use. Do not re-upload other creators' videos without permission.
