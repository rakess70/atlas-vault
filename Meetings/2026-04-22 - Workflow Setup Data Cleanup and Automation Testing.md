---
date: 2026-04-22
attendees: Bellwether Marketing
fathom_id: 140249469
fathom_url: https://fathom.video/share/hFzvSSk7xTLeFtkGNhVEzjy9kxody7Ba
type: meeting
---

# Workflow Setup, Data Cleanup, and Automation Testing

**Date:** 2026-04-22 | **Duration:** unknown
**Attendees:** Bellwether Marketing
**Fathom:** [View Recording](https://fathom.video/share/hFzvSSk7xTLeFtkGNhVEzjy9kxody7Ba)

## Summary
### [Data verification and workflow overview @ 0:00](https://fathom.video/calls/647548024?tab=summary&timestamp=0)

Ben begins by reviewing data pulling from Planning Center, noting concerns about hub groups and PCOS information accuracy. The team identifies three core next steps for the workflow: Renewing Commitment, Salvation, and Want to be Baptized. They filter out irrelevant items like "Not Ready to Commit" (an abandoned Easter initiative) and "Outreach/Go Team" additions that don't represent actionable next steps. Ben plans to schedule a meeting with the data owner to clarify the data source and ensure proper integration.

### [Process queues and conditional routing architecture @ 2:47](https://fathom.video/calls/647548024?tab=summary&timestamp=167)

The team discusses the technical structure of their workflow system, distinguishing between processes (the overall workflow) and queues (steps within a process that have been triggered but not yet fired). The Explore workflow uses conditional routing: when someone completes Explore Step 3 and scans a QR code, they fill out a form with team options (Worship Team, etc.), and each button press routes them to a specific team's process queue. Each step (1, 2, 3) has an associated form that collects information and triggers automation. The "Want to be a Member" flag appears when someone completes Explore Step 1, though the team questions whether this label accurately reflects the action.

### [Email template and mail merge configuration @ 5:24](https://fathom.video/calls/647548024?tab=summary&timestamp=324)

The team works through setting up email templates with mail merge capabilities. They discover that mail merge fields (like {{first\_name}}) can be inserted into email templates through the Communications section, but not directly in form confirmation pages. They create a confirmation email template that will be sent when someone completes a form, with the goal of personalizing messages using data from the form submission. The team explores whether mail merge works at the form level versus the process queue level, ultimately determining that templates need to be created separately in Communications and then referenced in the automation.

### [Baptism workflow setup and automation testing @ 19:35](https://fathom.video/calls/647548024?tab=summary&timestamp=1175)

Ben and Rod build out the "Want to be Baptized" process queue with two key steps: a confirmation email (sent immediately upon form completion) and an info email (providing baptism details). They reorder the queue to place confirmation first, select "Selected People" as the recipient type to ensure emails go to the person registering rather than their parent/primary contact, and save the template. When testing the workflow by submitting a test form, they discover the confirmation email requires manual sending rather than firing automatically—a significant limitation that means someone must manually trigger emails from the process queue rather than having them send automatically upon form submission.

### [Pushpay profile management and data cleanup task @ 33:24](https://fathom.video/calls/647548024?tab=summary&timestamp=2004)

Ben brings Iah Fernandez into the meeting to assign a data management task. The church uses Planning Center as their source of truth and needs to review Pushpay/CHMS accounts to identify and resolve duplicate and pending profiles. Iah initially has trouble accessing the account but successfully resets the password. Ben explains that pending profiles are people who created accounts or were imported from Planning Center, and the team needs to verify these are active, current members. Duplicate profiles occur when the same person has multiple accounts and need to be merged rather than ignored to maintain data integrity.

### [Duplicate profile merging process and examples @ 39:00](https://fathom.video/calls/647548024?tab=summary&timestamp=2340)

Ben walks Iah through the duplicate profile resolution process using real examples. For pending profiles, if information matches Planning Center records, they simply approve the profile. For duplicates, they must merge accounts while selecting the correct information—keeping the most recent/updated data and ensuring the active profile status is preserved. Examples include: Avery David (merging old and new records, keeping updated ID number), Ursula Bell/Harvey (recognizing a husband-wife pair where one registered the other, checking family relationships, and merging duplicate accounts), and profiles with conflicting data sources (giving records vs. signup records). The key principle is that merging prevents duplicate records in the system, whereas ignoring creates two separate records.

### [Action items and next steps @ 50:26](https://fathom.video/calls/647548024?tab=summary&timestamp=3026)

The team assigns clear next steps: Iah will begin with pending profiles first, then move to duplicate profiles, with support available from Ben and Rod as needed. Rod (Bellwether Marketing) will build out the remaining processes and queues, experiment with automation configurations, and troubleshoot the mail merge issue. Ben will research process queue automation by reviewing an article and video that Rod is sending, then report back on findings. The team plans to reconvene after Ben completes the research to determine the best approach for achieving fully automated email sending without manual intervention.


## Action Items
(none extracted)

## Follow-ups Needed
(none)

## Notes
