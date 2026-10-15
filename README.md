# The Critical Doc — with Dr Dan

An independent critical care education website created by Daniel Antonious, MD.
Brand domain: **thecriticaldoc.com**.

## Publish this complete folder on GitHub Pages

1. Extract `dr-dan-github-upload.zip` on your computer.
2. Create a GitHub repository (for example, `dr-dan-critical-care`).
3. Open **Add file → Upload files** and upload the **contents** of the extracted
   folder. `index.html` must be at the repository root, beside `clinical-images`
   and `scan-data`. Upload the folders with their contents; do not upload the ZIP
   as a replacement for the extracted files. Keep every filename unchanged.
4. Commit the uploaded files to `main`.
5. In the repository, open **Settings → Pages**. Under **Build and deployment**,
   choose **Deploy from a branch**, select **main** and **/ (root)**, then Save.
6. Wait for the Pages deployment to finish. Open the website URL shown there.
   For a project repository the URL normally follows
   `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.

GitHub supports browser uploads up to 25 MiB per file and 100 files at a time.
Every file in this package is below 8 MiB. If an upload is interrupted, upload
the missing files before enabling Pages. GitHub Desktop can also publish this
entire directory. No npm installation, build command or Git LFS is required.

If your Mac hides `.nojekyll`, use Command–Shift–period in Finder to show it,
or create an empty file named `.nojekyll` at the repository root using GitHub.
This bypasses Jekyll processing for the already-built website.

## Required website files

- `index.html`: complete app code, styling, question bank, creator portrait and
  scan metadata. This is the entry page.
- `clinical-images/`: 67 actual clinical image files used by the lessons.
- `scan-data/`: all nine included CT/MRI studies and supplied anatomy masks,
  split into small script parts and loaded when selected. Parts must stay together.
- `.nojekyll`: serves the existing HTML and assets directly on GitHub Pages.

`README.md`, `VALIDATION.md` and `ASSET-MANIFEST.json` document this release.
`.gitignore` excludes common desktop metadata. Keep them in the repository.

Do not upload the separate 130 MB standalone HTML or a website ZIP into the
repository as the entry page. The extracted files here are the deployable site.

## Connect thecriticaldoc.com after purchase

Keep the GitHub Pages URL working while you register the domain. After you own
and verify the domain in GitHub, add `thecriticaldoc.com` in **Settings → Pages →
Custom domain**, configure the DNS records shown in the official guide, and
enable HTTPS when GitHub makes it available. The package intentionally has no
active CNAME redirect: setting a name before it belongs to you would make the
initial GitHub Pages preview harder to verify.

Domain and DNS guide: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Features and stored progress

The site includes diagnosis and procedure guides, embedded clinical images,
scrolling scan viewers, bronchoscopy exploration and quiz, ventilator teaching
and simulation, ECG rhythms, device tracings, microbiology, research and 600
original critical care board-style questions. Learning mode is untimed and
shows explanations after each answer. Timed mode withholds them until review.

Progress is stored on the same browser/device using localStorage and a small
functional returning-visitor cookie. This release does not provide server-based
accounts, a password login or cross-device synchronization. Export/import in
Board Review provides a manual progress backup.

Research refresh uses a public Europe PMC API and requires an internet
connection. The local teaching images and included scans do not require their
original publishers' servers. Other links open their credited source pages.

Anatomy names are supplied by paired source segmentations or small teaching
landmarks placed on the exact included examination. A landmark is not a whole-
organ segmentation. Unannotated points are identified as unannotated. An exam
with known pathology is not presented as a normal reference.

## Review before broad public promotion

See `VALIDATION.md` for the checks performed and their limits. This educational
site and original question bank are independent of ABIM and are not official
exam questions or a prediction of examination performance.

Clinical content and simulator output require Daniel Antonious, MD's editorial
review. Verify the deployed website on Safari/Chrome and a phone before sharing
it widely; automated source/event-model checks are not a full browser audit.

## Source credits and reuse

Credits and reuse terms accompany the clinical figures and each included study
inside the site. These third-party assets retain their individual terms. In
particular, the CHAOS abdominal MRI retains CC BY-NC-SA 4.0 conditions, and the
automated aortic segmentation is identified as an uncorrected source mask.
There is no blanket open-source license applied to third-party images or data.

## Official publishing references

- https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
