# Design Spec: Replace Forks Badge with Profile Views Badge

## Objective
Replace the forks badge in the `README.md` file with a profile views counter badge that preserves the exact colors, size, and style (red/black, `for-the-badge` style, same height) but changes the text and counter logic to show profile views.

## Scope of Changes
- Target file: `README.md`
- Target block: Lines 14-19 (Forks badge `<a>` and `<img>` tags).
- Modifications:
  - Update `alt` and `title` to "Profile Views".
  - Update `src` parameter `label` to "Profile Views".
  - Update `src` logo to `eye`.
  - Update target URL to use the dynamic JSON badge endpoint pointing to `https://views.igorkowalczyk.dev/api/json/muhamadgalihsaputra`.
  - Update badge `width` attribute from `111px` to `165px` to match the new text length without squishing/stretching.
  - Update the link `href` of the badge to the user's profile `https://github.com/muhamadgalihsaputra`.
