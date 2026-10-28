# Patterns for destructive actions

A destructive action is anything that removes or alters a resource in a way that can’t be easily recovered. Examples include deleting a document, canceling an account or withdrawing a FOIA request.

Some destructive actions aren’t obvious: Redactions in DocumentCloud are one-way and can’t be undone. Reprocessing a document potentially alters it. 

In all of these cases, we need to confirm the user’s intent and give them a chance to cancel the action before proceeding.
