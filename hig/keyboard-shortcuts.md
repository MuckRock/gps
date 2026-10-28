# Keyboard shortcuts

Keyboard shortcuts are a power user feature, meant to speed up an otherwise mouse-driven workflow, not to replace it.

Keyboard shortcuts should stick to common patterns and browser conventions:

- Escape cancels an action or closes a modal.
- Enter and Space on a focused button or anchor clicks it.
- Arrow keys navigate or scroll.

Don’t override existing browser functions, unless you have a very good reason. Cmd-F (or Ctrl-F) already searches the current page. To use our search, use Cmd-K (as is becoming standard elsewhere).

We should document keyboard shortcuts for ourselves and for users, but we can do that on a dedicated page. Sometimes it’s nice to have a tooltip or a specific shortcut highlighted in a form.

## Tab navigation

Never use keyboard shortcuts in a way that breaks browser accessibility features, like tab navigation.

When defining interactive elements, ensure that they use appropriate tab indexes for ordering.
