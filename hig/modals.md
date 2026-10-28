# Modals

Modals are useful when you need to take an action without leaving the current page. These should be focused actions – edit a document’s metadata, confirm deletion – and not something that needs a URL of its own.

Modals should not open based on URL state, only a user action on the page. If a URL configures how a page behaves, the page should handle that.

The user should always have a clear path to closing the modal, and it should be clear what closing the modal does.

![Modal for editing a document’s access settings, with Save, Cancel and close buttons](img/modals-close-options.png)

This modal can be closed in four ways:

- Clicking “Save” will change the document’s access settings.
- Clicking “Cancel” will close the modal without saving.
- Clicking the X in the top right corner will close the modal without saving.
- Hitting the Escape key will close the modal without saving.

Every modal will support the last two options: an explicit close button in the top right, using the circled X icon, and the Escape key.

## Nesting modals

We almost never nest modals. Only nest when an action within the modal requires a step outside the main workflow, and only if there isn’t a better solution.

![A create-project modal nested on top of the add-to-project modal](img/modals-nested.png)

In this case, I wanted to add a document to a project and then decided to create a new project in the process. That opened a second, nested modal on top of the modal to select projects. When I close this modal, I’ll go back to the first.
