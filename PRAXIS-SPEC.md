# PRAXIS --- Master Production Specification

> **Turn your experience into your professional identity.**

## Purpose

PRAXIS is a next-generation resume, CV, portfolio, and career-document
studio.

It must feel like a professional **career-document operating system**,
not a simple "fill out a form and download a PDF" website.

The user enters professional information once, stores it locally, and
creates multiple professional documents from the same master profile.

Supported document types should include:

-   Resume
-   CV
-   Internship Resume
-   Academic CV
-   Portfolio
-   Cover Letter
-   Professional Bio
-   Achievement Sheet
-   Reference Sheet
-   Digital Professional Card

------------------------------------------------------------------------

# 1. Non-Negotiable Architecture

PRAXIS MUST be deployable entirely through **GitHub Pages** as a **100%
static, client-side web application**.

## Do NOT require

-   Node.js backend
-   Express
-   PHP
-   Python backend
-   Java backend
-   Firebase
-   Supabase
-   MongoDB
-   MySQL
-   PostgreSQL
-   Authentication server
-   REST API
-   GraphQL server
-   Server-side rendering
-   Custom backend
-   Server-side database

## Allowed technologies

Use:

-   HTML
-   CSS
-   JavaScript
-   IndexedDB
-   LocalStorage
-   Service Worker
-   Web APIs
-   Client-side libraries where appropriate

A user must be able to deploy the repository directly to GitHub Pages.

If a build tool is used, the final output must remain compatible with
static GitHub Pages hosting.

------------------------------------------------------------------------

# 2. Branding

## Product name

**PRAXIS**

## Primary tagline

**Turn your experience into your professional identity.**

## Supporting direction

**Build. Design. Export. Apply.**

Create a clean professional PRAXIS wordmark/logo using HTML/CSS/SVG
rather than relying on copyrighted external assets.

------------------------------------------------------------------------

# 3. Design Philosophy

The visual identity must communicate:

-   Confidence
-   Precision
-   Professionalism
-   Seriousness
-   Technical sophistication
-   Trust
-   Career growth
-   User control

## Squared-edge visual language

The default interface must use:

-   `0px` border radius
-   Thin borders
-   Strong typography
-   Clean grids
-   High contrast
-   Precise spacing
-   Minimal decorative elements
-   Professional monochrome foundation
-   Controlled accent colors

Do NOT make the application look like a generic SaaS dashboard full of
oversized rounded cards.

Small radius values may be offered as an optional setting, but **0px
must be the default**.

The application should feel like a professional design/document tool.

------------------------------------------------------------------------

# 4. Responsive Workspace

## Desktop

Use a professional three-region workspace:

``` text
┌─────────────────────────────────────────────────────────┐
│ PRAXIS                         SAVE ●       PROFILE     │
├──────────────┬─────────────────────┬───────────────────┤
│ NAVIGATION   │ EDITOR              │ LIVE PREVIEW      │
│              │                     │                   │
│ Profile      │ Section editor      │ Resume page       │
│ Education    │                     │                   │
│ Experience   │                     │                   │
│ Projects     │                     │                   │
│ Skills       │                     │                   │
│ Design       │                     │                   │
│ Settings     │                     │                   │
├──────────────┴─────────────────────┴───────────────────┤
│ Undo │ Redo │ Zoom │ Fit │ Print │ PDF │ Fullscreen    │
└─────────────────────────────────────────────────────────┘
```

## Tablet

Use a two-panel editor/preview interface.

## Mobile

Use:

``` text
Header
Editor
Preview
Bottom Navigation
```

Bottom navigation:

-   Home
-   Edit
-   Design
-   Preview
-   Settings

------------------------------------------------------------------------

# 5. Theme Engine

Support:

-   Auto
-   Light
-   Dark
-   OLED

Auto must follow the operating-system preference using
`prefers-color-scheme`.

## Accent colors

Provide:

-   Professional Blue
-   Royal Purple
-   Emerald
-   Teal
-   Crimson
-   Orange
-   Monochrome
-   Custom

Use CSS variables for dynamic theming.

Application UI theme and resume design theme must be independently
configurable.

------------------------------------------------------------------------

# 6. Resume Editor

Create a powerful section-based editor.

## Sections

-   Personal Information
-   Profile Photo
-   Professional Summary
-   Education
-   Work Experience
-   Internships
-   Projects
-   Skills
-   Certifications
-   Awards
-   Publications
-   Languages
-   Volunteer Work
-   Organizations
-   Interests
-   References
-   Custom Sections

Every section must support:

-   Add
-   Edit
-   Delete
-   Duplicate
-   Hide / Show
-   Reorder
-   Drag & Drop

Provide keyboard-accessible alternatives to drag-and-drop.

------------------------------------------------------------------------

# 7. Master Profile

Create a central **MASTER PROFILE**.

The user enters information once.

``` text
MASTER PROFILE
├── Personal Information
├── Education
├── Experience
├── Internships
├── Projects
├── Skills
├── Certifications
├── Awards
├── Publications
├── Languages
├── Volunteer Work
├── Organizations
└── Custom Data
```

Use this master profile to create multiple documents:

-   Software Engineer Resume
-   Cybersecurity Resume
-   Internship Resume
-   Academic CV
-   Portfolio

------------------------------------------------------------------------

# 8. Multiple Documents and Versions

Allow multiple local documents.

Example:

``` text
MY DOCUMENTS

Software Engineer
Updated today

Cybersecurity
Updated yesterday

College Internship
Updated 3 days ago

Academic CV
Updated last week
```

Each document can independently control:

-   Template
-   Sections
-   Section order
-   Content
-   Typography
-   Layout
-   Colors
-   Visibility

------------------------------------------------------------------------

# 9. Template Engine

Build a reusable template engine.

Do NOT hardcode a single resume.

Templates must consume a common structured resume-data schema.

## Professional

-   Classic
-   Corporate
-   Executive
-   Minimal

## Technology

-   Software Engineer
-   Cybersecurity
-   Developer
-   Data / AI

## Student

-   Student
-   Fresher
-   Internship

## Academic

-   Academic CV
-   Research

## Creative

-   Modern
-   Portfolio

New templates must be addable without rewriting the core engine.

------------------------------------------------------------------------

# 10. Design Studio

Create a dedicated Design Studio.

Controls:

-   Template
-   Layout
-   Typography
-   Colors
-   Spacing
-   Margins
-   Header
-   Footer
-   Sections
-   Profile Photo
-   Icons
-   Links
-   Page Settings

------------------------------------------------------------------------

# 11. Layout Engine

## Columns

-   Single Column
-   Two Column
-   Left Sidebar
-   Right Sidebar

## Page size

-   A4
-   Letter
-   Legal
-   Custom

## Orientation

-   Portrait
-   Landscape

## Margins

-   Compact
-   Normal
-   Wide
-   Custom

## Spacing

-   Tight
-   Balanced
-   Relaxed
-   Custom

------------------------------------------------------------------------

# 12. Typography Engine

Allow customization of:

-   Font family
-   Font size
-   Heading size
-   Line height
-   Letter spacing
-   Font weight
-   Section heading style

Use legally appropriate/open-source fonts when bundling fonts.

Possible professional fonts:

-   Inter
-   Roboto
-   Lato
-   Source Sans
-   IBM Plex Sans
-   Georgia
-   Times New Roman
-   System fonts

------------------------------------------------------------------------

# 13. Geometry / Shape System

Default corner radius:

``` text
0px
```

Optional:

``` text
0px
2px
4px
8px
12px
```

Also support:

-   Border thickness
-   Divider thickness
-   Shadow intensity
-   Section separators

------------------------------------------------------------------------

# 14. Live Preview and Render Engine

Every meaningful modification must update the resume preview without a
page reload.

Architecture:

``` text
USER INPUT
   ↓
STRUCTURED STATE
   ↓
VALIDATION
   ↓
TEMPLATE ENGINE
   ↓
RENDER ENGINE
   ↓
LIVE PREVIEW
```

The preview must represent the actual printable document rather than a
separate approximation.

------------------------------------------------------------------------

# 15. Zoom and View Controls

Provide:

-   50%
-   75%
-   100%
-   125%
-   150%
-   Zoom In
-   Zoom Out
-   Fit Width
-   Fit Page
-   Fullscreen Preview
-   Page navigation

------------------------------------------------------------------------

# 16. Multi-Page Document Engine

Support professional multi-page resumes and CVs.

Handle:

-   Page breaks
-   Section breaks
-   Margins
-   Headers
-   Footers
-   Page numbers
-   Content overflow
-   Orphan headings
-   Excessive whitespace

Never allow:

-   Content overlap
-   Text clipping
-   Broken layout

Avoid splitting logical sections unnecessarily.

------------------------------------------------------------------------

# 17. Print System

Create a dedicated Print Studio.

Controls:

``` text
Paper: A4
Orientation: Portrait
Margins: Normal
Scale: 100%

[ PRINT ]
[ SAVE AS PDF ]
```

Use:

``` css
@media print
```

and dedicated print CSS.

The printed result should closely match the preview.

When printing, hide all application UI and output only the document.

------------------------------------------------------------------------

# 18. Client-Side PDF Engine

Implement client-side PDF generation.

Support:

-   A4
-   Letter
-   Multi-page PDF
-   Correct margins
-   Page breaks
-   Fonts where technically feasible
-   PDF metadata
-   Professional file names

Example:

``` text
Anish_Kushwaha_Resume.pdf
```

PDF generation must not require a backend.

------------------------------------------------------------------------

# 19. Resume Health / Document Check

Create a deterministic local diagnostic engine.

Do NOT claim to predict hiring outcomes or employer decisions.

Check for:

-   Missing contact information
-   Missing education
-   Missing experience
-   Missing skills
-   Empty sections
-   Very short descriptions
-   Excessive page count
-   Excessive whitespace
-   Poor formatting
-   Missing links
-   Inconsistent dates
-   Inconsistent formatting
-   Possible duplicate entries

Example:

``` text
PRAXIS CHECK

Profile              ✓
Education            ✓
Experience           ✓
Projects             ✓
Skills               ✓
Contact              ✓
Formatting           ✓
Content Density      ⚠
Consistency          ✓

12 checks passed
2 suggestions
```

------------------------------------------------------------------------

# 20. Content Guidance

For experience and project sections, provide structured local guidance:

``` text
What did you do?

What tools or technologies did you use?

What was your contribution?

What was the result?

Can you quantify the result?
```

Provide examples/templates locally.

Do not require an AI API.

Do not fabricate achievements.

The user remains responsible for the truthfulness of their content.

------------------------------------------------------------------------

# 21. Achievement Builder

Create an achievement editor based around:

``` text
ACTION
+
SKILL / TECHNOLOGY
+
RESULT
+
MEASURABLE IMPACT
```

Provide optional local writing templates.

------------------------------------------------------------------------

# 22. Project Builder

Fields:

-   Project Name
-   Description
-   Role
-   Technologies
-   Contribution
-   Results
-   GitHub URL
-   Live Demo URL
-   Start Date
-   End Date

Support technology tags and multiple projects.

------------------------------------------------------------------------

# 23. Education Builder

Fields:

-   Institution
-   Degree
-   Field
-   Board / University
-   Start Date
-   End Date
-   Grade / CGPA / Percentage
-   Relevant Coursework
-   Achievements
-   Description

Every field should be hideable when unnecessary.

------------------------------------------------------------------------

# 24. Experience Builder

Fields:

-   Company
-   Role
-   Location
-   Employment Type
-   Start Date
-   End Date
-   Current Position
-   Responsibilities
-   Achievements
-   Technologies

Support multiple bullet points and multiple positions.

------------------------------------------------------------------------

# 25. Profile Photo Studio

Client-side image tools:

-   Upload
-   Crop
-   Resize
-   Rotate
-   Zoom
-   Position
-   Square
-   Circle
-   Hide photo

Do not upload photos to a server.

------------------------------------------------------------------------

# 26. QR Code Generator

Allow client-side QR generation for:

-   GitHub
-   LinkedIn
-   Portfolio
-   Personal website
-   Public resume URL

QR generation must happen locally.

------------------------------------------------------------------------

# 27. Link Handling

Recognize and validate URLs for:

-   GitHub
-   LinkedIn
-   Portfolio
-   Personal website
-   Email
-   Phone

Render them professionally in templates.

------------------------------------------------------------------------

# 28. Undo / Redo

Implement:

``` text
Ctrl + Z → Undo
Ctrl + Y → Redo
```

Also provide visible toolbar controls.

Maintain a reliable history stack without excessive memory usage.

------------------------------------------------------------------------

# 29. Autosave

Automatically save meaningful changes locally using debounced
persistence.

Display:

``` text
Saving...
Saved locally ✓
```

Do not create unnecessary writes for every keystroke.

------------------------------------------------------------------------

# 30. Storage Architecture

## IndexedDB

Use for:

-   Resume documents
-   Master profile
-   Versions
-   Drafts
-   Application tracker
-   Local assets

## LocalStorage

Use for:

-   Theme
-   UI preferences
-   Last opened document
-   Zoom
-   Lightweight settings

Avoid storing sensitive information unnecessarily.

------------------------------------------------------------------------

# 31. Privacy Center

Create a **Privacy Center** explaining the actual architecture.

Example:

``` text
PRAXIS processes your resume locally
in your browser for the core application.

No account is required for the core experience.
```

Provide:

-   Export All Data
-   Import Backup
-   Delete All Local Data

Do not make privacy claims that the implementation cannot guarantee.

------------------------------------------------------------------------

# 32. Backup System

Provide:

``` text
Export PRAXIS Backup
Import PRAXIS Backup
```

Example:

``` text
PRAXIS_Backup_YYYY-MM-DD.json
```

Include:

-   Profiles
-   Documents
-   Settings
-   Versions
-   Metadata

Do not include unnecessary secrets.

------------------------------------------------------------------------

# 33. Import / Export

## Import

-   PRAXIS JSON
-   JSON profile
-   Markdown where practical
-   Plain text where practical

## Export

-   PRAXIS JSON
-   JSON
-   Markdown
-   HTML
-   TXT
-   PDF

------------------------------------------------------------------------

# 34. Command Palette

Implement:

``` text
Ctrl + K
```

Commands:

-   Create new resume
-   Add experience
-   Add project
-   Change template
-   Open Design Studio
-   Export PDF
-   Print
-   Toggle Dark Mode
-   Open Settings
-   Import backup
-   Export backup
-   Open Privacy Center

Support keyboard navigation and search.

------------------------------------------------------------------------

# 35. Keyboard Shortcuts

At minimum:

``` text
Ctrl + S       Save
Ctrl + Z       Undo
Ctrl + Y       Redo
Ctrl + P       Print
Ctrl + K       Command Palette
Esc            Close dialog
```

Avoid breaking normal browser shortcuts when inappropriate.

------------------------------------------------------------------------

# 36. PWA

Create:

``` text
manifest.json
sw.js
```

Support:

-   Installable app
-   Offline shell
-   Cached application assets
-   Offline templates
-   Local data
-   App icon
-   Splash screen
-   Standalone mode

Use a robust service-worker caching strategy.

Do not place private user data into public/shared caches unnecessarily.

------------------------------------------------------------------------

# 37. Offline-First

After the required application assets are cached, PRAXIS should continue
working without network access.

Offline capabilities:

-   Editing
-   Preview
-   Design
-   Local saving
-   Printing
-   PDF generation
-   Import/export
-   Version history

Architecture:

``` text
Browser
   ↓
Service Worker
   ↓
Cached PRAXIS
   ↓
IndexedDB
   ↓
Resume Engine
```

------------------------------------------------------------------------

# 38. Career Document Suite

Use the Master Profile to generate:

-   Resume
-   CV
-   Cover Letter
-   Professional Bio
-   Portfolio
-   Reference Sheet
-   Achievement Sheet
-   Internship Resume
-   Academic CV
-   Digital Professional Card

All documents should share the same structured data model.

------------------------------------------------------------------------

# 39. Job Application Tracker

Create a completely local application tracker.

Fields:

-   Company
-   Role
-   Location
-   Application Date
-   Status
-   Job URL
-   Notes
-   Interview Date
-   Follow-up Date

Statuses:

-   Saved
-   Applied
-   Interview
-   Offer
-   Rejected
-   Withdrawn

No external job-platform integration is required for the core product.

------------------------------------------------------------------------

# 40. Career Dashboard

Create a professional dashboard showing locally calculated metrics.

Example:

``` text
WELCOME BACK

Career Profile
────────────────────

Resume Versions       4
Projects              12
Skills                24
Certifications        7
Applications          16

Profile Completion     92%
Document Checks        86%

Recent Activity
────────────────────
Updated Resume
Added Project
Created CV
```

------------------------------------------------------------------------

# 41. Smart Local Assistant

Create a deterministic local assistant.

Example:

``` text
PRAXIS ASSISTANT

I noticed:

⚠ Your summary is empty.
⚠ Your project descriptions are very short.
✓ Education is complete.
✓ Contact information is complete.

Suggestions:

[Review Summary]
[Review Projects]
[Check Formatting]
```

Do not fabricate facts.

Do not pretend this is an AI model.

------------------------------------------------------------------------

# 42. Custom Section Builder

Allow users to define their own sections.

Example:

``` text
Section: Open Source Contributions

Fields:
• Project
• Contribution
• Date
• Link
• Description
```

The template engine must render custom sections.

------------------------------------------------------------------------

# 43. Design System

Create centralized CSS variables:

``` css
--bg
--surface
--surface-2
--text
--text-muted
--border
--accent
--danger
--success
--warning
--radius
--shadow
```

Default:

``` css
--radius: 0px;
```

Avoid scattering hardcoded styles across components.

------------------------------------------------------------------------

# 44. Accessibility

Implement:

-   Semantic HTML
-   Keyboard navigation
-   Visible focus states
-   Screen-reader labels
-   ARIA only where needed
-   Accessible dialogs
-   Accessible dropdowns
-   Keyboard alternative to drag/drop
-   Reduced motion
-   High contrast
-   Proper form labels
-   Accessible error messages
-   Touch-friendly controls

Support:

``` css
prefers-reduced-motion
```

------------------------------------------------------------------------

# 45. Performance

PRAXIS must feel fast.

Requirements:

-   Avoid unnecessary dependencies
-   Lazy-load heavy functionality
-   Debounce autosave
-   Avoid excessive DOM re-rendering
-   Efficient IndexedDB usage
-   Avoid layout thrashing
-   Optimize PDF generation
-   Optimize image processing
-   Cache static assets
-   Keep initial load small

Do not sacrifice correctness for premature micro-optimization.

------------------------------------------------------------------------

# 46. Security

Because PRAXIS handles personal professional information:

Implement:

-   Strict input validation
-   Safe HTML rendering
-   Avoid unsafe `innerHTML` where unnecessary
-   Sanitize user-generated markup
-   Validate imported JSON
-   Limit imported data sizes
-   Validate URLs
-   Prevent script injection
-   Never execute imported code
-   Avoid unnecessary third-party trackers
-   Avoid exposing private data in URLs unnecessarily

Never use:

``` js
eval()
```

Never execute user-provided JavaScript.

------------------------------------------------------------------------

# 47. No Telemetry by Default

Do not add analytics, advertising trackers, or telemetry by default.

If analytics are ever added in the future, make them clearly optional
and document them.

------------------------------------------------------------------------

# 48. Error Handling

Create professional error states.

Example:

``` text
Something went wrong while rendering this document.

[ Retry ]
[ Restore Previous Version ]
```

For invalid imports:

``` text
This PRAXIS backup could not be loaded.

The file may be invalid or corrupted.

[ Choose Another File ]
```

One malformed entry must never crash the entire application.

------------------------------------------------------------------------

# 49. Empty States

Make empty states useful.

Example:

``` text
NO PROJECTS YET

Projects can demonstrate what you can actually build.

[ + Add Project ]
```

------------------------------------------------------------------------

# 50. Confirmation Dialogs

For destructive actions:

``` text
Delete this resume?

This action cannot be undone.

[ Cancel ] [ Delete ]
```

Deleting all local data must require explicit confirmation.

------------------------------------------------------------------------

# 51. File Naming

Generate safe professional names:

``` text
Name_Resume.pdf
Name_CV.pdf
Name_Portfolio.pdf
PRAXIS_Backup_YYYY-MM-DD.json
```

Sanitize filenames safely.

------------------------------------------------------------------------

# 52. Print Quality

The resume must be suitable for real-world printing.

Check:

-   A4 dimensions
-   DPI-independent layout
-   Print margins
-   Text sharpness
-   Page breaks
-   Background handling
-   Link formatting
-   Font fallback
-   No clipped content
-   No accidental UI elements

When printing, hide all editor/UI controls.

------------------------------------------------------------------------

# 53. Preview Quality

The preview should visually represent the actual document.

Use a page-like canvas with:

-   Page background
-   Page shadow
-   Zoom
-   Page navigation
-   Multi-page support

Do not allow preview-only UI to leak into exported documents.

------------------------------------------------------------------------

# 54. Mobile Experience

On mobile:

-   Make preview scrollable
-   Provide fullscreen preview
-   Provide clear editing controls
-   Keep touch targets comfortable
-   Keep bottom navigation accessible
-   Make Print/PDF actions easy to reach
-   Never require desktop-only interactions

------------------------------------------------------------------------

# 55. Recommended Project Structure

``` text
PRAXIS/
├── index.html
├── builder.html
├── preview.html
├── css/
│   ├── core.css
│   ├── editor.css
│   ├── themes.css
│   ├── print.css
│   └── responsive.css
├── js/
│   ├── app.js
│   ├── editor.js
│   ├── renderer.js
│   ├── templates.js
│   ├── storage.js
│   ├── pdf.js
│   ├── print.js
│   ├── history.js
│   ├── validation.js
│   ├── command-palette.js
│   └── pwa.js
├── templates/
│   ├── professional/
│   ├── modern/
│   ├── ats/
│   ├── student/
│   └── academic/
├── assets/
├── manifest.json
├── sw.js
├── README.md
└── PRAXIS-SPEC.md
```

------------------------------------------------------------------------

# 56. Data Model

Design a versioned structured data schema.

Suggested top-level model:

``` json
{
  "schemaVersion": 1,
  "profile": {},
  "documents": [],
  "settings": {},
  "history": [],
  "applications": []
}
```

Keep the schema extensible.

Write migration functions for future schema versions.

The data model must be independent of the editor UI and templates.

------------------------------------------------------------------------

# 57. Architecture Principles

Keep these layers independent:

``` text
UI
 ↓
Application State
 ↓
Data Model
 ↓
Validation
 ↓
Template Engine
 ↓
Document Renderer
 ↓
Print/PDF Engine
```

Do not tightly couple template markup to form components.

A template should be able to consume structured profile data without
knowing how the editor works.

------------------------------------------------------------------------

# 58. Quality Requirements

Test:

-   Desktop Chromium
-   Firefox
-   Safari where practical
-   Android browsers
-   Responsive layouts
-   Offline mode
-   PDF export
-   Print preview
-   Multi-page documents
-   Import/export
-   IndexedDB persistence
-   Backup restore
-   Corrupted JSON handling
-   Keyboard shortcuts
-   Accessibility
-   Dark/light/auto themes
-   Mobile interactions
-   Empty states
-   Long resumes
-   Very short resumes
-   Large profile photos
-   Unicode names and content
-   Special characters
-   Long URLs
-   Multiple documents
-   Version restore

------------------------------------------------------------------------

# 59. GitHub Pages Deployment

The final project must work from a normal GitHub Pages repository.

Asset paths must work correctly when the repository is hosted under a
GitHub Pages **project path**, not only at the root domain.

If using a build system, provide a static build/deployment workflow
compatible with GitHub Pages.

Prefer a dependency-light architecture.

Include clear deployment instructions in `README.md`.

------------------------------------------------------------------------

# 60. Implementation Instructions for Codex

You are not being asked to create a visual mockup.

**Build the actual functional application.**

Do not leave major functionality represented by placeholder buttons.

Do not silently introduce a backend.

Do not replace functional features with screenshots or fake
interactions.

Use modular, maintainable JavaScript.

Keep the UI polished and production-grade.

Use progressive enhancement where practical.

Ensure the application can recover gracefully from malformed local data.

Use accessible semantic HTML.

Keep the resume rendering engine independent from the editor UI.

Keep the data model independent from individual templates.

Keep print/PDF rendering separate from application chrome.

Make the application extensible so additional templates and document
types can be added without rewriting the core engine.

If a feature cannot be implemented exactly under a static GitHub Pages
architecture, implement the closest genuinely functional client-side
alternative and clearly document the limitation.

Do not remove a requested feature merely because it is complex. Break
complex features into maintainable modules and implement them
incrementally.

------------------------------------------------------------------------

# 61. Final Acceptance Criteria

PRAXIS is complete only when a user can:

1.  Open the site on GitHub Pages.
2.  Create a master professional profile.
3.  Create a resume without an account.
4.  Add, edit, delete, hide, duplicate, and reorder sections.
5.  See changes instantly in a live preview.
6.  Change template.
7.  Change theme.
8.  Change layout.
9.  Change page size.
10. Change typography.
11. Change spacing and margins.
12. Change geometry/shape settings.
13. Upload and crop a profile photo locally.
14. Create multiple resume versions.
15. Undo and redo changes.
16. Automatically save locally.
17. Close and reopen the browser without losing saved documents.
18. Work offline after the application is cached.
19. Export/import a PRAXIS backup.
20. Export PDF locally.
21. Print professionally.
22. Generate multiple pages correctly.
23. Run document-quality checks.
24. Use keyboard shortcuts.
25. Use the command palette.
26. Install the PWA.
27. Use the application on mobile.
28. Delete all local data.
29. Create additional document types from the same master profile.
30. Deploy the entire application using GitHub Pages only.

------------------------------------------------------------------------

# 62. Final Product Standard

PRAXIS must feel like a serious production application, not a school
project or a static form.

The overall product architecture should resemble:

``` text
                         PRAXIS
                           │
                ┌──────────┴──────────┐
                │                     │
             PROFILE              DOCUMENTS
                │                     │
       ┌────────┼────────┐      ┌─────┼─────┐
       │        │        │      │     │     │
    Skills   Projects  Career  Resume  CV  Portfolio
                                    │
                              ┌─────┴─────┐
                              │           │
                           DESIGN       EXPORT
                              │           │
                       ┌──────┼──────┐    │
                       │      │      │    │
                     Theme  Layout  Type  PDF
                       │      │      │    │
                       └──────┼──────┘    │
                              │           │
                         PRINT / SAVE / SHARE
```

## Core product principles

-   Static-first
-   Offline-first
-   Local-first
-   Privacy-conscious
-   User-controlled
-   Professional
-   Accessible
-   Fast
-   Extensible
-   GitHub Pages compatible

**Build PRAXIS as a real, polished application---not a demo.**
