# Dassatek website

A complete static HTML5, CSS3 and JavaScript website. No backend, framework, npm, Node.js, or installation is required to view or host it.

## Preview

Open `index.html` in your browser. All main content is already in HTML, so it remains readable without JavaScript. Search, mobile navigation and video playback use JavaScript. Google Forms and YouTube require internet access; some browsers restrict embeds on local file URLs, so verify them again on your live HTTPS domain.

## Publish on Hostinger

1. Open your website’s file manager in Hostinger and go to `public_html` (or the document root shown for your domain).
2. Back up any existing website before replacing its files.
3. On your computer, open `tools/publish.html`. Enter your real HTTPS website address and select **Download updated pages**. Extract that ZIP into this website folder and allow it to replace the generated pages and config file. This adds canonical URLs and a sitemap using your domain.
4. Upload the `.html` files, `assets` folder, `robots.txt`, and generated `sitemap.xml` into the domain’s document root. `index.html` must sit directly in that root, not inside another Dassatek folder.
5. Keep `tools`, this guide, and `CONTENT-NOTES.md` on your computer. They do not need to be public.
6. Enable HTTPS for the domain. Open the homepage, navigation, form, videos and a blog article on desktop and mobile.
7. Submit the sitemap URL to your search engine webmaster accounts if you use them. Hosting and domain access remain under your control; this package does not deploy itself.

No SMTP or email-hosting setup is required. Contact submissions go to your Google Form.

## Project structure

- `index.html`: homepage with the supplied illustrated cover.
- `about.html`, `our-work.html`: brand story and five areas of work.
- `initiative-*.html`: Awakening Young Farmer and Roots & Canopy.
- `knowledge.html`, `resource-*.html`: searchable knowledge archive and source-linked resources.
- `blog.html`, `blog-*.html`: separate Blog and full articles.
- `video.html`: featured podcast and all supplied episodes.
- `get-involved.html`: Google Form, email, and contact options.
- `privacy.html`, `404.html`: privacy and error pages.
- `assets/css`: responsive styling and locally served fonts.
- `assets/images`: supplied logos, optimized photos, and podcast thumbnails.
- `assets/documents`: the supplied public U.S. Mission project highlight.
- `assets/js/config.js`: contact details, social URLs, domain, and Google Form URL.
- `assets/js/projects.js`: all initiative data.
- `assets/js/posts.js`: all blog post data.
- `assets/js/resources.js`: all Knowledge Hub content.
- `assets/js/videos.js`: all podcast data and verified metadata.
- `assets/js/render.js`: shared publishing templates; normally leave unchanged.
- `assets/js/main.js`: menu, search, filters, animations, and video playback.
- `tools/publish.html`: browser-based HTML publisher; no installation needed.

## Add or edit content

1. Open the matching data file in a plain-text editor. Duplicate an existing entry and replace its content. Keep quotes, commas, and brackets valid.
2. Give every new item a unique lowercase slug using hyphens. Keep established slugs unchanged to preserve links.
3. Add images to `assets/images`. Blog, project and resource image names refer to a base name; provide `NAME-640.webp` and `NAME-1280.webp` versions. For example `my-farm-640.webp` and `my-farm-1280.webp` use `my-farm` in the data. Existing images can be reused.
4. Use real publication dates and correct authors. Do not use publication dates to imply historical reporting that did not occur.
5. Open/reload `tools/publish.html` and export the updated pages. This regenerates overviews, details, search metadata, structured data, and (when a domain is entered) sitemap from the central data files.
6. Extract and upload the updated HTML, edited data files, and new images. Data-only edits do not automatically change the already-published static HTML: the export step is necessary to keep search engines and visitors seeing the same content.
7. If deleting an article or changing a slug, also remove/redirect its old HTML file on your host.

Video entries use a YouTube ID, real title, date, thumbnail, description, topic, ISO 8601 duration, and featured flag. The current episodes share one topic; category filters appear automatically when multiple video topics are introduced. Unavailable players retain a visible Watch on YouTube link.

## Google Form settings

The supplied form opens publicly without a sign-in prompt in the retrieved public view. It currently asks for Name, Email, Address (required), optional Phone number, and Comments.

Recommended owner settings:
- Keep Name and Email required, and require a useful enquiry/Comments field.
- Consider making Address optional: an exact address is usually unnecessary for a first enquiry.
- Add Organization and Interest (partnership/funding/research/learning/other) if useful.
- Enable email-format response validation for Email.
- Ensure responder access allows your intended public audience. Turn off organization restrictions and “Limit to 1 response” if they force sign-in. Avoid file-upload questions if you need submissions without sign-in.
- Use a confirmation such as: “Thank you for contacting Dassatek. We’ve received your enquiry and will get back to you.” Do not promise a response time you cannot meet.
- Limit response-sheet and form-editor access to your team. Do not enable public response summaries.
- In Responses, enable email notifications for new responses. Optionally link responses to a private Google Sheet.
- Submit one real test enquiry yourself after publishing and check receipt. No test response was sent on your behalf.

The form provides its own validation, submission handling, and confirmation. The website cannot customize or detect the internal state of a cross-origin Google Form. Its visible alternative link and email address remain available if embedding fails.

## Search and accessibility

Pages include unique titles and descriptions, semantic headings, Open Graph and Twitter text metadata, relevant structured data, keyboard focus, skip navigation, responsive layouts and reduced-motion support. The site intentionally has no invented production-domain URL. Enter your real domain with the publishing helper before launch to generate canonical URLs and the sitemap.

There are no promised rankings or AI citations. Knowledge summaries link to their sources. Article and video content is present in static HTML. Uploaded logo colors guide the palette; bright yellow is an accent, with dark text for readability.

## Fonts

Manrope, Source Sans 3, and Kantumruy Pro are served locally. All Khmer text uses Kantumruy Pro. Font families are distributed under the SIL Open Font License; see `assets/fonts/OFL-*.txt`.
