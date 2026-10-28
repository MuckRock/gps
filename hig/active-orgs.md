# “Active” orgs and teams

Several products use a concept of an “active” organization. This may go away in the future, and while it exists, it’s something of an anti-pattern.

Currently, both DocumentCloud and MuckRock allow a user to set an active organization.

![Active organization menu in DocumentCloud](img/active-orgs-documentcloud.png)

![Active organization menu in MuckRock](img/active-orgs-muckrock.png)

In DocumentCloud, a user’s active organization affects uploading, premium access and credit usage.

Every document is owned by an organization (including individual organizations). A user’s active org at the time of upload becomes the document’s owning organization. This can be changed later, but it’s considered a destructive action, since it can affect users’ access to a document.

If an organization has a premium subscription, members of that organization can access premium features. Switching to a non-premium organization means a user loses access to those features.

Finally, certain add-ons require spending “AI credits” (this name may change). We bill those credits against the organization’s account.

On MuckRock, organizations have an allotment of requests, plus premium features.

We count requests against an organization’s budget, and switching organizations changes which account we deduct requests from. Premium features work the same as on DocumentCloud.

The current system is opaque and can lead to users accidentally uploading to or filing requests under the wrong organization. Choosing an active organization is hidden under a navigation menu that users may not see.

In the future, we’d like to allow users to choose organizations when taking an action. For example, when uploading a document, a user should be able to choose which organization owns it, defaulting to the most recent used. Similarly, when filing a FOIA request, the user should choose the organization to bill against.
