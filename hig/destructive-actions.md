# Patterns for destructive actions

A destructive action is anything that removes or alters a resource in a way that can’t be easily recovered. Examples include deleting a document, canceling an account or withdrawing a FOIA request.

Some destructive actions aren’t obvious: Redactions in DocumentCloud are one-way and can’t be undone. Reprocessing a document potentially alters it. 

In all of these cases, we need to confirm the user’s intent and give them a chance to cancel the action before proceeding.

![Confirmation dialog before reprocessing a document](img/destructive-actions-confirm-reprocess.png)

![Confirmation dialog before deleting a document](img/destructive-actions-confirm-delete.png)

![Confirmation dialog before saving redactions](img/destructive-actions-save-redactions.png)

![Confirmation dialog before discarding a redaction](img/destructive-actions-discard-redaction.png)
