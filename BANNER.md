# GitHub profile banner

The README contains desktop and mobile banner images. A `<picture>` element selects the portrait layout on screens up to 640 px wide. Both images link to the portfolio.

- `assets/bio-banner.webp`: desktop export, 1800 × 940.
- `assets/bio-banner-mobile.webp`: mobile export, 1000 × 1160.
- The matching `.svg` files are editable, self-contained sources. Text, colors, geometry and portrait placement can be changed in an SVG editor. Export the matching WebP again after editing.

The design uses Asith's existing signature from [his portfolio](https://asith.cc/), a GitHub-dark background, and original geometric artwork inspired by the supplied reference. Name, role, bio and links were checked against the [portfolio About page](https://asith.cc/about.html).

## Show this on the main profile

GitHub requires a public repository with the same name as the account. For this account, the repository must be `asithc/asithc`, with `README.md` at the root.

In this repository's **Settings → General → Repository name**, change `My-Github-repo` to `asithc` and click **Rename**. Keep it public and keep the README on the default branch. The relative image paths continue to work after renaming.

See [GitHub's profile README instructions](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme).

## Portrait source and processing

The portrait comes from Asith's existing [public GitHub profile photo](https://avatars.githubusercontent.com/u/7944580?v=4). Its background was removed with the built-in imagegen tool. Typography and geometric layout were assembled separately as SVG and exported to WebP in a browser.

Final imagegen prompt:

> Use case: background-extraction. Edit target: the supplied photograph of Asith wearing an olive outdoor jacket, blue mirrored sunglasses and a black headband beside a blue lake. Create a precise transparent cutout of ONLY this exact man, including his hair, headband, sunglasses, face, olive jacket, arms, hands and visible torso through the bottom crop. Remove all scenery: mountains, sky, blue lake and other background. Preserve the subject's exact identity, original face, expression, proportions, pose, clothing, lighting and colors. Do not retouch, beautify, redraw or invent new body portions. Preserve the original bottom crop. Use genuine alpha transparency outside the subject, with clean natural edges. No backdrop, no shadows added, no text. This will be placed over a dark GitHub bio banner.

## Validation

Desktop and mobile previews were checked at 1280 px and 390 px. Both loaded the expected image and had no horizontal overflow. The SVG sources were checked for XML parse errors. The final exports preserve transparent rounded corners.
