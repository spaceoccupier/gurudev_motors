# Homepage Refinements

## Scope

The local preview was reviewed and approved on 2026-10-11. The user requested publishing these changes to `spaceoccupier/gurudev_motors` and updating the existing public Vercel preview link. Keep the deployment in sample mode.

- Mobile hero: following the user's refinement, keep the name on the left and price on the right. Tighten the heading spacing and move this row upward, reserving clear sky below it so the landmarks do not overlap the text. Preserve the full background, separate vehicle motion and controls.
- Desktop hero: remove the solid background from the engine, fuel and gears list. Keep mobile's existing details strip.
- Search: use the full inner content width, aligned with the categories below.
- Inside Gurudev Motors: replace the four-photo collage with a reserved founder portrait, founder message and two existing showroom photos, followed by one wide, blank team-photo placeholder. Stack portrait, message and photos on phones.

## Founder Content

Use Rajesh Sharma only as an explicitly labelled example name. Mark the entire message as sample content and make no factual claims about the real founder. Suggested example message: We want choosing a vehicle to feel simple. Tell us what you need, and we will help you compare your options, understand the price and find what suits you.

The team photograph is not available. Reserve a landscape area labelled Team photo, without inventing staff or using a stock group picture. Keep the gallery page and its full photo collection unchanged. Existing showroom photos still open in the accessible photo viewer.

The user also requested a cutout-style founder photo and then confirmed to keep it blank for now. Reserve a portrait area labelled Founder photo, with no invented person or stock portrait. A supplied photo can later be background-removed and placed in that area.

## Verification

Check 320, 360, 390, 600, 768, 1024, 1440 and 1920 pixel widths. Verify the model row stays above both landmark zones and the vehicle, search edges match the content, the new section has two photos and empty portrait and landscape areas, the viewer supports keyboard and close controls, and there is no horizontal overflow. Run showroom and road-hero tests, TypeScript and lint. Capture local screenshots for review before publishing.

## Local Verification Completed

- All eight viewport widths checked, with no horizontal overflow and matching search/category edges.
- All five brands checked at 320 pixels: heading, model and price remain separate, with text above the clock-tower landmark region.
- Founder layout has two real showroom photos, an empty portrait area and an empty landscape team-photo area. The separate gallery collection still has four photos.
- Photo viewer moves to the second photo, wraps to the first, traps backwards tab focus, closes with Escape and restores trigger focus.
- Searching Honda opens `/vehicles?q=Honda` and shows two matching sample vehicles.
- All 18 showroom/road-hero tests pass. TypeScript and targeted component lint pass. No browser console errors observed.
- Screenshots: `docs/qa/hero-raised-row-mobile.png`, `docs/qa/founder-preview-desktop.png`, `docs/qa/founder-preview-mobile.png` and `docs/qa/homepage-refinements-desktop.png`.
- Local review completed. Publishing is authorized to the existing `preview/hero-framing` branch and `gurudev-motors-preview.vercel.app` alias; deployment verification follows the build.
