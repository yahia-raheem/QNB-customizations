# Description

- Client wants to create a new categorization on each personnel in `CTM:People`
- The categorization will be on the same level as the department of each user
- The cat. is used to determine a list of approvers (approvers per cat.) that will approve a set of SRDs that are going to be created on the environment
- The cat. approvers will also be marked as approvers in the `CTM:People` form
- In case any approver or any one belonging to the new categorization has either their `Department`, `Organization`, `title`, or `Site` change, then they will be removed from the categorization and their approver flag should be reset (removed as approver).
  - Also, an email with this change should be sent to the `user authorization team` telling them of the change
- A new form will be created where the new categorization entries will be submitted
  - The new form will include a name, and status, fields.
- Initially, Marian will input the data for each user to be included for the new cat., and whether he's an approver or not in `CTM:People`
- A new SRD will be created to allow a user to select a cat. and user to add/remove as approver of the cat.
  - Entitilement of this should be limited to the `user authorization team`
- A new SRD will be created to allow a user to select a cat. and a user to add/remove him/her to the categorization (this is to allow the user to submit tickets on the target SRDs).
- All end user SRDs will have entitlement so that only users that belong to one of the new categorization are allowed to submit these requests.
