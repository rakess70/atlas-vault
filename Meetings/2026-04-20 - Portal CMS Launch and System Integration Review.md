---
date: 2026-04-20
attendees: Bellwether Marketing
fathom_id: 139363468
fathom_url: https://fathom.video/share/aozJC7njKtCSDLwVyf5MnqaJkzpFqB3a
type: meeting
---

# Portal CMS Launch and System Integration Review

**Date:** 2026-04-20 | **Duration:** unknown
**Attendees:** Bellwether Marketing
**Fathom:** [View Recording](https://fathom.video/share/aozJC7njKtCSDLwVyf5MnqaJkzpFqB3a)

## Summary
### [Portal Content Management System Launch @ 0:52](https://fathom.video/calls/644033284?tab=summary&timestamp=52)

Rod demonstrated a new Content tab in the portal that streamlines content creation and management. The system allows users to create content entries by selecting month/year, topic, page type (new/rewrite/update/expand), and assigning writer and publisher roles. Each entry includes optional fields for target keywords and topic notes. The interface displays character counts and word counts in real-time, with autosave functionality ensuring no work is lost. Users can upload and manage image galleries with individual alt text and notes for each image.

### [Content Review and Approval Workflow @ 2:23](https://fathom.video/calls/644033284?tab=summary&timestamp=143)

Once content is submitted for review, it moves through a multi-stage approval process. Topics first enter a "pending" stage where clients can approve or request changes via their portal interface. After topic approval, content moves to a "writing" stage where team members add meta titles, descriptions, H1 titles, and primary keywords. Once content is complete, it's submitted for a second review where approvers can approve or request changes. Upon final approval, the content is marked as published with an assigned URL, and both team members and clients receive notifications with links to view the live page.

### [Three-Tier Access System and Notifications @ 16:41](https://fathom.video/calls/644033284?tab=summary&timestamp=1001)

The portal implements three distinct access tiers: Team (full access), Client (Bellwether staff), and Customer (end clients). Customers access their portal via magic links on a subdomain (e.g., ecb.seo.teamaccess.agency) without requiring login credentials. The system sends automated email notifications at each workflow stage, and includes real-time collaboration indicators showing which team members are currently working on specific pages to prevent conflicts. Tim and Rod discussed the option of generating brand-neutral PDFs for clients to forward to their end customers, though this would add overhead.

### [Content System Integration with Tasks @ 20:53](https://fathom.video/calls/644033284?tab=summary&timestamp=1253)

Rod raised a question about whether content items should also appear in the tasks section, since they currently only show in the Content tab. Tim noted that for SEO projects, content does show as repeating tasks in the workflow, but the team acknowledged they need to refine how content integrates with the task system. They discussed potentially creating a "Publish Monthly Content" task that links directly to the Content tab, allowing team members to access content details without leaving the task view. Rod noted this integration work can be refined once they implement recurring content workflows.

### [Stripe Subscription Metadata Improvements @ 27:19](https://fathom.video/calls/644033284?tab=summary&timestamp=1639)

Rod implemented improvements to Stripe subscription tracking. Going forward, SEO subscriptions will automatically include the client site name in the subscription label and metadata, allowing better tracking of which payment corresponds to which project. Rod manually updated existing subscriptions (e.g., Gutter Concepts) and corrected renewal dates (e.g., setting one to renew on the 25th). This enhancement improves billing clarity and financial tracking across multiple client projects.

### [Code Review Feedback and Security Findings @ 37:05](https://fathom.video/calls/644033284?tab=summary&timestamp=2225)

Pat Hurst provided technical feedback after reviewing a Loom video of the app (he has not yet accessed the app directly). He expressed excitement about the system and requested the ability to test and run a project through the workflow. Pat identified several technical issues:
• **Non-critical items**: HasBugs in seedproduction.js (dev tooling only), API tenants patch with no field whitelist (admin route only), and various cosmetic/legacy code issues
• **Security concern**: The RentCast API endpoint lacks authentication and could allow unauthorized API calls if the URL is discovered, potentially burning through API credits. Rod noted this should be fixed eventually but is not urgent since the app is not yet in production.

### [Portal PRD Compliance and Remaining Features @ 48:12](https://fathom.video/calls/644033284?tab=summary&timestamp=2892)

Rod reviewed the portal's Product Requirements Document against the actual code implementation. Most features are tracking well. Current gaps include:
• Website folder contents are created but read-only listing inside the portal isn't functioning
• Remaining features to implement: SEO results dashboard with AI chat, team calendaring, SOP and library, time tracking, and advanced reporting
• Lead gen workflow needs refinement (minor, workflow-related rather than infrastructure)
Rod noted these are not major blockers and the system is nearly ready for full deployment.

### [External Inquiry and Meeting Recap @ 51:04](https://fathom.video/calls/644033284?tab=summary&timestamp=3064)

Rod received a text from Josh Green (Rush Remodeling lead gen client) asking whether to use Perplexity Platform instead of ChatGPT, claiming Perplexity provides access to the latest ChatGPT version. Rod will respond to clarify that Perplexity only offers access to older OpenAI 4.0 model, not the latest versions. Tim expressed strong satisfaction with the content management system, calling it "the missing piece" that brings everything under one roof. He thanked Rod for the extensive work completed in a short timeframe and noted the system will keep everyone in the loop throughout the content workflow.


## Action Items
(none extracted)

## Follow-ups Needed
(none)

## Notes
