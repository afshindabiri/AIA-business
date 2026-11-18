# AiA Business: Claude Code start here

This private repository is the business and website requirements reference, not the verified application checkout, deployment target, or a fork of Dots.

## Read first

1. [README.md](README.md) for scope, navigation, and source status.
2. [Website handoff](archive/source-dots/topics/aia-website/CLAUDE-CODE-HANDOFF-2026-11-16.md) for sitemap, service pages, the two start paths, and first preview goals.
3. [Questionnaire checkpoint](archive/source-dots/topics/aia-business/questionnaire-checkpoint-2026-11-14.md) to separate approved questionnaires from drafts.
4. [Portal decisions](archive/source-dots/topics/aia-business/approved-questionnaire-client-portal-decisions-2026-11-07.md) for intake, request numbers, and approval/version rules. Prefer later explicit owner corrections when they conflict with older records.
5. [Source manifest](SOURCE-MANIFEST.json) for exact originals, associated projects, and gaps. Provenance may refer to the private Dots repository; do not assume those links are required to open the included copies.

## First task for the website

Inspect the actual website checkout, branch, remote and working-tree state read-only first. Do not assume this documentation repository is that checkout. Verify its identity and existing assets before proposing code changes; if it is unclear, prepare the plan/content only and clarify the application repository instead of inventing one. This guide and the documentation migration do not authorize a build, deployment or integration now.

The initial visual preview is **the Persian RTL homepage and one complete AI Reception service page**, not a bilingual launch. English localization is later. When preview work is authorized, use a reversible branch or separate local preview, with illustrative data and nonfunctional forms/chat. A two-page wireframe, Persian copy and a readable process diagram on desktop and mobile are enough for this first review. Show it to Afshin before expanding to the other services, connecting real services or publishing. Check availability of Taste and UI/UX Pro Max in the target Claude session; do not assume they are installed.

## Design discretion and preview checks

Proposed structure, tools, sequence, copy and wireframes are starting points, not fixed implementation choices. Within authorized local preview work, improve unapproved technical and design choices reversibly when there is a better approach; record the reason and how to test it. Do not silently change business facts or confirmed owner decisions. This discretion is not permission for unapproved installations, persistent settings, external integrations or publication.

Discoverability priority is **GEO first by a wide margin, then AEO, then SEO**. Make the title, service description and response/handoff stages readable in HTML. In the future local preview, check these contents and their order with JavaScript disabled, alongside RTL, mobile readability, keyboard navigation, main links/buttons and reduced-motion behavior. Animation must clarify the story; the diagram must also work without motion. These are acceptance checks to perform, not checks already passed or a guarantee of search/AI placement.

## AI Reception: show the actual decision branches

Use a recognizable illustrative workflow: business problem → customer input → checking verified business information → the permitted response or escalation branch → customer-visible outcome. Each node should make its input, action and output clear; an n8n-like visual does not mean every solution uses n8n. Do not imply existing client deployments.

For the example “Do you serve my area?”:
- If coverage is known in the verified reference **and automatic response is authorized**, answer the coverage question, then ask the service type needed to register the request.
- If coverage is unknown or the case needs review, do not invent a coverage answer or prematurely imply a service request can proceed. Hand the question, area and available details to the responsible human.
- In draft mode, a human sends the message. In reminder mode, the system does not answer the customer.

Choose channels and languages only after checking needs and feasibility. Telephone support is optional and the customer supplies a compatible telecom service. These examples describe product behavior, not authority to contact a real customer now.

## Intake, customer confirmation and AiA acceptance

Keep navigation freely accessible. Begin the start-of-cooperation request with name, business field, role, phone and WhatsApp; keep consultation and service requests distinct. Do not add email or preferred time to this five-field initial request form. The pinned handoff identifies distinct fields for consultation booking and website-chat-to-WhatsApp referral. Do not merge the separate website-chat-to-WhatsApp referral flow with this initial request form; follow the pinned handoff's three data paths.

Service questionnaires are short, conditional and completed/edited only in the customer portal, with one identified respondent and role. The checkpoint distinguishes approved forms from drafts; limited approved amendments do not approve an entire draft. Each service request has a unique number, but that number is not authentication or access permission.

1. Before submission, show the completed answers to the customer for review and explicit confirmation. The first answer set becomes **v1 when the customer confirms it**, still pending AiA review.
2. Every version, including v1, becomes the reference only after **separate AiA review and acceptance**. This is not a commitment to implement every answer.
3. Edits to the latest pending version retain its number. After AiA accepts a version, subsequent changes create the next version, with differences visible.
4. The last accepted version remains the reference until its replacement is accepted. Keep project/request status separate from questionnaire-review status.

## Domain and context-specific links

The owner's intended primary domain is **aiafshin.com**; **afshin.ae** is the other domain. This is not evidence of present site availability and does not authorize DNS, redirects or deployment. Preserve older statements about domain uncertainty or publication status as historical source text rather than silently editing the archive.

Owner-supplied AiA channels, kept distinct by context and language:
- AiA LinkedIn: https://www.linkedin.com/in/aiafshin
- Persian Instagram: https://www.instagram.com/aiafshin.ae/
- English Instagram: https://www.instagram.com/aiafshin.uae/
- Persian Telegram: https://t.me/AiAfshin_ae
- English Telegram: https://t.me/AiAfshin_uae

The separate résumé contact link is https://www.linkedin.com/in/afshindabiri/. It does not replace the AiA link by implication. Before actual footer publication, verify both exact LinkedIn targets and final redirects in an ordinary signed-out browser, and resolve any remaining intended-destination ambiguity before adding a cross-link. Current profile contents/redirects are not verified here. An indexed profile headline is not confirmation of identity linkage. This list is handoff context, not approval to build or publish a footer, change profiles, schedule posts or conduct outreach.

## Boundaries

Do not deploy, enable live intake, migrate client data, change DNS, reset, overwrite working assets, or add dependencies/settings without the separate authority appropriate to that action. Mark unresolved product and pricing choices as unresolved; keep captured historical sources unchanged. Do not read all source archives into prompts by default. Consult relevant files for each task. The authored guidance above incorporates later owner clarifications without modifying the pinned historical evidence.
