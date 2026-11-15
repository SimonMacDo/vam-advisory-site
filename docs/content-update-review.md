# Controlled content update — Vera review

Prepared 15 November 2026 on `content/vera-controlled-update-2026-11-15`, based on main commit `1df0576bb90eebec01a20734cb0ea2581811ff1e`.

## Scope and sources

Read both supplied Word documents in full and extracted the copy directly from their paragraphs and tables:

- `VAM_Advisory_Website_Copy_Recommendations_Aligned.docx`
- `Toby Wai - Bio for VAM.docx`

The explicit page-copy blocks are implemented within the existing HTML/CSS layout. Explanatory recommendations, new client-wordmark sections, navigation changes, SEO and launch instructions are not treated as approval to redesign or publish.

## Pages

| Page | Change |
| --- | --- |
| `/` | Supplied hero, introduction, six service previews, case feature and founder copy; Vera's name, title, photograph and dedicated founder section retained. |
| `/services/` | Supplied six service sections and training copy, in the document's explicit order. Legal documentation remains first, as it already was on main. Existing litigation representation note retained. |
| `/case-studies/` | Supplied introduction and four case narratives; no invented outcomes or named-client attribution. |
| `/team/` | Supplied heading/introduction; existing Vera, Todd and Konrad cards retained in order; Toby appended as member four. |
| `/team/vera-tan/` | Supplied subheading, opening, background, corresponding experience wording and closing; existing founder title, photo and other background retained. |
| `/team/toby-wai/` | New profile with the complete four-paragraph biography verbatim and supplied Senior Legal & Compliance Adviser title. No photograph or invented synopsis. |
| `/contact/` | Supplied contact heading, introduction, email copy and button; existing contact details retained. |
| `/team/todd-james/`, `/team/konrad-li/` | Shared footer and closing-section copy only; individual biographies, roles and photographs unchanged. |

All nine pages use the supplied footer descriptor and, where a closing section exists, its supplied heading, body and “Speak with VAM” button. Navigation, typography, colours, CSS, image files, URLs and existing metadata are unchanged. The new Toby page has a descriptive name/title and retains staging indexing restrictions.

## Content comparison and deliberate exceptions

| Source | Staging result / difference |
| --- | --- |
| Explicit body copy, service descriptions and Toby biography | Copied directly from Word, with no paraphrasing, punctuation corrections or added claims. 88 selected block comparisons passed exact text equality; all newly introduced visible strings were also checked against the documents or existing site text. |
| Word layout | HTML escapes ampersands and lays out paragraphs responsively. Browser rendering collapses repeated spaces and replaces Word pagination/line wrapping. No words are changed by this conversion. |
| Home service cards | All six supplied entries use existing service-row styling; numeric prefixes are separate elements. The original preview showed four entries. |
| Services order | Uses the six explicitly numbered sections in the document; legal documentation was already first and remains first. No independent service categories were added. |
| Founder home heading | “Vera Tan” and her existing title remain prominent. Supplied “Senior judgment, built in.” occupies the existing lead/subheading position. |
| Founder profile title and experience | Existing “Founder & Managing Partner” retained rather than changing the title to the document's “Founder and Managing Partner.” Existing AGBA historic role, role descriptions and background-source note retained because their removal is not explicitly directed. |
| Case-page label | Document contains “Successful Cases”, “Success Cases”, “SUCCESS CASES” and “Success Cses”. Existing navigation “Case studies” and page eyebrow “Selected case studies” retained pending a decision; explicit home feature wording is used as supplied. |
| Client names and wordmarks | Proposed new client section omitted pending approval; no names attributed to individual cases and no logos added. Existing generic case-client labels were removed where the new anonymous case narratives supersede them. |
| People-page explanatory paragraph | The unlabelled Vera/Toby recommendation is not inserted as additional public copy. Labelled heading/introduction implemented; existing lead and all three existing team cards preserved. |
| Buttons and navigation | Page-specific “Explore our services”, “Meet Vera”, “View success cases” and “Email VAM” used where supplied. Existing navigation labels and profile contact buttons preserved. Global “Speak with VAM” applied to closing sections only. |
| Staging notices / launch checklist | Existing review banners, including “October 2026”, and approval notices retained. Instructions to remove them for a public launch were not applied. |
| SEO recommendations | Not implemented. No SEO audit, title/description rewrite, sitemap update, indexing change or production configuration change. |

## Decisions/assets for Vera

1. Supply an approved Toby photograph if one should be shown. His title and relationship to VAM are explicitly supplied in his biography and require no invention.
2. Choose the final case-page/navigation label; confirm whether “Success Cses” is a typo to correct.
3. Confirm whether to add the proposed named-client section and approve any client wordmark assets.
4. Existing Todd and Konrad role/association confirmation notices remain; their current approved titles should be confirmed before launch.
5. If desired, approve corrections to source wording such as “kyc”, “Spac”, “regulatory compliant” and “Close findings and implementation…”. These were not silently corrected.
6. Confirm whether the existing historic AGBA role and accompanying founder-profile details should remain. They have been preserved under the controlled-update instruction.

## Validation and deployment boundary

- Exact source-copy comparisons passed; every introduced visible string was traced to supplied copy or retained site text.
- All internal links, fragment anchors and referenced local assets resolve, including the new Toby route.
- Vera remains the first team member, the only founder, and the home-page featured person.
- Existing CSS and photographs are byte-for-byte unchanged; existing Todd and Konrad biographies are text-identical.
- Desktop browser review at approximately 1348 px; mobile rendering checked in 390 px frames (375 px content area). All nine pages fit without horizontal overflow. This is browser responsive testing, not physical-device testing.
- Team photographs and logo successfully load in the browser.
- No tracked deployment configuration or GitHub Actions workflow exists in the inspected tree. README describes GitHub Pages publishing main; this update does not change main or Pages settings.
- The revised site was served in an internal review preview. No persistent shareable branch-preview URL was provisioned or verified. The draft pull request is the durable review result.
- No merge, production deployment, live-site write, DNS, hosting or email configuration change was made. The original live website was not modified by this work.

Do not merge or publish as a production launch without the separately requested review and approval.
