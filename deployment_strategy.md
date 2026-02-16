# Strategic Deployment & Admin Plan: "JUNE" Landing Page

## 1. Executive Summary
The goal is to move the "JUNE" landing page from a prototype to a production-ready system that is **Fast (Astro)**, **Secure (Microsoft Auth)**, and **Low-Maintenance (AWS Amplify)**.

**Recommendation**: Deploy on **AWS Amplify** and implement a **Headless Admin** portal secured via **Microsoft Entra ID (Azure AD)**.

---

## 7. Professional Content Workflow: UAT vs. Production

This is one of Keystatic's strongest advantages over WordPress. It uses **"Gated Publishing"** based on Git branches.

### A. The "Staging" Workflow
1.  **Create a UAT Branch**: We set up a branch called `uat` or `staging` in GitHub.
2.  **AWS Integration**: AWS Amplify creates a "Preview URL" (e.g., `uat.june.trexo.com`) that automatically syncs with this branch.
3.  **Keystatic Admin**: The marketing team logs in and selects the "uat" branch in the dropdown.
4.  **Edit & Review**: They make changes and click "Save". These changes are live **only** on the UAT URL for internal review.

### B. The "Publish to Prod" Workflow
Once the CEO or Marketing Manager approves the UAT site:
1.  **Git Merge**: You (or the developer) merge the `uat` branch into the `main` branch.
2.  **Instant Deploy**: AWS Amplify detects the merge and deploys the approved content to the production site (`june.trexo.com`) in ~2 minutes.

### C. Advanced: "Drafts" via Pull Requests
Keystatic allows non-technical users to create **Draft Branches** directly from the UI.
*   Marketing clicks "New Branch" -> "Spring_Campaign_Hype".
*   They edit the site.
*   They click **"Submit for Review"** inside the Keystatic UI.
*   This creates a **GitHub Pull Request**. A manager can see exactly what changed (word-for-word) before allowing it to go live.

---

## 2. Infrastructure Costs at Scale: "What if it Goes Viral?"
(Previous content preserved...)

## 3. Scalability for Content: Blogs, Partners, and Clients
(Previous content preserved...)

## 4. Maintainability: Site vs. Admin
(Previous content preserved...)

## 5. Security & Threat Protection (DDoS & Bots)
(Previous content preserved...)

## 6. Final Verdict & Next Steps
(Previous content preserved...)
