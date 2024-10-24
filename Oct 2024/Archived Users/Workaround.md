# Workaround
Displayed an error message to archived users on submitting a ticket. The message is `You are Not Authorized to use the system. Please send email to Marian Jan, Lamiss RAMADAN, and Yassmine YASSIN for assistance.`

# Steps
- Created a custom field named `Requester Account Status` in the `SRM:Request` form.
- Created a new filter named `INT.Enable_Archived_Profiles` to set the value of `Requester Account Status` from `CTM:People`
  - Set the filter `Execution Order` to `1`
- Created a new filter named `INT.Error_Incaseof_Archived_User` to Display an error to the user in case of his/her profile status is `Archive`
  - Set the filter `Execution Order` to `2`