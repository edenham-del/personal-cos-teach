Skip this command entirely if you don't have an expense/approval tool
connected — it's optional.

Read config.yaml from this folder.

Steps:
1. Get recent transactions for the user.
2. Get pending requests to review.
3. Get reimbursements awaiting approval.
4. Get bills awaiting approval.

Present:
- Pending approvals table (type, from, amount, age)
- Flag anything over alert_threshold (config.yaml, default $5000)
- Note auto-approvable items (under auto_approve_below, default $500)

If the request I gave you asks to approve something specific, use the appropriate
approve action.

the request I gave you
