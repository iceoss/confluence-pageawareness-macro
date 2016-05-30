# Macros
| File                           | Name                           | Title                         |
| ------------------------------ | ------------------------------ |------------------------------ |
| pageawareness.vm               | pageawareness                  | Page Awareness                |
| pageawareness-summary.vm       | pageawareness-summary          | Page Awareness Summary        |
| pageawareness-userlist.vm      | pageawareness-userlist         | Page Awareness User List      |
| pageawareness-globalstatus.vm  | pageawareness-globalstatus     | Page Awareness Global Status  |

# Page Awareness Macro
The page awareness macro adds functionality to confluence pages allowing for acknowledgement, review and approval of page content. Each of which is tied directly to the version of the specific page, and is automatically invalidated if the page changes. This is useful for pages such as corporate policies where various staff are responsible for reviewing the content of a page, approving the policy and then requiring other users to acknowledge they are aware of the policy.

This macro has two modes, Interactive and Status. This is controlled by the Status Mode parameter when adding the macro to a page. When in interactive mode the macro will check if the logged in user is responsible for review or approval of the page. If they are, it will display a simple bar indicating the users responsibility and providing a button to mark their acknowledgement. If the user is not assigned to review or approve the page they are presented with a bar and button allowing them to acknowledge the content of the page. If the page is later changed, all acknowledgements, reviews and approvals will be disregarded and the review / approval / acknowledgement process starts again.

When status mode is set to "Yes". The macro simply display a status indicator. The indicator is relevant only to that user indicating the status of the page. If the user is assigned to review or approve the page, and they ave not acknowledged the latest version of the page, a "TODOS" status will be displayed. Otherwise, it will display the state of the page. Note: When status mode is set to Yes - the assigned user details will be read from the first page awareness macro and therefore do not need to be re-entered in the status macro.

**Interactive Mode Screenshots:**

![Acknowledge Page Content](resources/sample-acknowledge.png)
![Under Review](resources/sample-underreview.png)
![Reviewer](resources/sample-reviewer.png)
![Pending Approval](resources/sample-pendingapproval.png)
![Approver](resources/sample-approver.png)

**Status Mode Screenshots:**

![TODOS](resources/sample-status-todos.png)
![CHANGES](resources/sample-status-changes.png)
![UPTODATE](resources/sample-status-uptodate.png)
![APPROVED](resources/sample-status-approved.png)
![REVIEWED](resources/sample-status-reviewed.png)
![PENDING](resources/sample-status-pending.png)

# Page Awareness Summary Macro
The page awareness summary macro provides a table style list view of users who are assigned to review and/or approve the page, or a list of all users who have acknowledged the content of the page, including the version and date of their acknowledgement.

**Screenshots:** TODO

# Page Awareness User List
The page awareness user list macro is similar to the summary macro, however provides a comma delimited list of users useful for display in property grid tables.

**Screenshots:** TODO

# Page Awareness Global Status Macro
The global status macro is similar to the status mode display, but provides a global status relevant to all users viewing the page. If the page is pending review, the status will be "PENDING", if the page has been reviewed "REVIEWED", approved "APPROVED".

**Screenshots:** TODO
