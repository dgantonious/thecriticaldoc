# Release verification — v16

Checked on October 14, 2026 (America/New_York).

## Corrections in this release

- The Critical Doc identity appears in the shared navigation, page titles, home
  branding, footer and social metadata. The domain is displayed as intended branding.
- About the Creator is the last main navigation item. The original 1320 × 1630
  portrait bytes are retained with automatic height and contain sizing, without
  zoom, transforms, a forced aspect ratio or cropping.

- Bronchoscopy opening labels retain the same DOM buttons during continuous
  breathing. Long clicks and keyboard activation can complete before navigation.
- Tree nodes have larger transparent targets; withdrawal, quiz replay, camera
  movement and map position retain their existing continuous navigation model.
- Scan hover labels refresh under a stationary mouse after scrolling. Mouse,
  pointer and tap inspection are supported. Labels clear when leaving the image
  or loading another study. The pixel value remains tied to the displayed slice.
- A Find a structure control locates a real voxel of a supplied segmentation.
  Five CT studies without masks have 33 explicitly placed teaching landmarks.
  Their small neighborhoods are not represented as whole-organ segmentations.
- The creator portrait is limited to 200 px on desktop, 180 px on smaller screens
  and 172 px on phones. The caption sits below it, beside the biography on desktop.
- This GitHub package uses index.html and small scan parts. Original embedded
  image and mask byte hashes are preserved after reassembly.

## Automated checks

- 716 assembled-site route, control and markup checks; 386 rendered fragments.
- 29 board-review model and event checks; all 600 explanation panels and their
  3,000 answer explanations. Learning mode is untimed; timed tests defer feedback.
- 18 existing bronchoscopy, quiz, ventilator and lifecycle regression checks.
- 22 new interaction checks, including held clicks across breathing frames,
  every airway's withdrawal, stationary-pointer relabeling, source geometry,
  portrait constraints and annotations in all three planes of all nine volumes.
- Existing waveform checks, independent pressure/volume mechanics comparisons,
  actual-photo integrity checks and package/scan integrity checks were rerun.
- The GitHub package check verifies every scan part, source image/mask hashes,
  local clinical image mapping, entry-point syntax, relative URL resolution,
  successful and failed scan loads, and archive integrity.

## Limits of verification

These are automated Node/DOM/event-model and native-canvas checks. This runtime
has no installed browser executable, so real Safari/Chrome layout, pointer hit
routing, WebGL rendering and mobile-device behavior have not been verified here.
The sustained-click regression proves that animation no longer destroys the
control; it is not a claim of a completed end-to-end browser test.

No automated suite proves all educational content clinically correct. The
existing citations, drug content and simulator assumptions remain available for
Daniel Antonious, MD's editorial review. This bank is original educational
content, not official ABIM material or a validated prediction of board success.

The reported counts are suite checks; many checks exercise multiple structures,
questions, frames, planes or individual voxels. They are not independent patients.

## Check the deployed website

Open the published URL on Safari and Chrome, and on a phone. Confirm: every main
navigation tab; procedure steps and photographs; CT/MRI scrolling and named
anatomy; held clicks on breathing airway openings; withdrawal and quiz replay;
ventilator setting changes; ECG/device selections; untimed learning feedback;
timed submission; progress after reload; creator portrait; online research feed.
Keep index.html and all asset directories together when updating the deployment.
