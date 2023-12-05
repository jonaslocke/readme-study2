---
title:  Notice Full Summary
---

import FullNoticeImg from '@site/static/images/ms-telex-ui/full-notices-summary.png';

Notice Full Summary

<img src={FullNoticeImg} />

### HIX
- [HIX-174231](../HIX/HIX-174231)
- [HIX-174239](../HIX/HIX-174239)

### Tasks

#### HIX-174231
- Update Notice Delivery radio buttons to the following table below:

<table>
  <tr>
    <th>Current Label</th>
    <th>Description</th>
    <th>Proposed new label</th>
  </tr>
  <tr>
    <td>Secure inbox only - Send alert</td>
    <td>Sends alerts based on communication preferences</td>
	<td>Alerts</td>
  </tr>
  <tr>
    <td>Email - Do not send alert</td>
    <td>Sends notice by email only</td>
	<td>Email or Postal Mail</td>
  </tr>
  <tr>
    <td>SMS only</td>
    <td>Sends notice by SMS only</td>
	<td>SMS</td>
  </tr>
  <tr>
    <td>Use Recipient Communication Preference</td>
    <td>Uses communication preferences to determine whether to send via postal mail or which alert channels to use</td>
	<td>Recipient communication preferences</td>
  </tr>
  <tr>
    <td>Invitationy</td>
    <td>Sends notice by postal mail or email depending on client configuration. Exclusively used for invitation notices from Account Transfer or Easy Enrollment.</td>
	<td>Email and Postal mail</td>
  </tr>
  <tr>
    <td>Postal Mail only</td>
    <td>Sends notice via postal mail regardless of communication preferences.</td>
	<td>Postal Mail</td>
  </tr>
</table>


#### HIX-174239
- Create two new buttons on the Full Summary Component
	- Create “Delete (number#) queued notices” button and “Deactivate Template” button
	- Only visible if notices are queued. 
	- Buttons should not be exposed while notices are being regenerated. 
	- Clicking button will expose standard “Are you sure?” button. 
	- If no queued notices, don’t show “Delete queued notice” button.  This acts as both a confirmation that queued notices were deleted and keeps the UI clean. 
	- Decrease width of version module - giving more space back to “body” of template.


### User Stories / Unit Tests

#### HIX-174231
- Notice Full Summary buttons should display all of the following radio buttons:
	- Alerts
	- Email or Postal Mail
	- SMS
	- Recipient communication preferences
	- Email and Postal mail
	- Postal Mail

#### HIX-174237
- User should be able to view English and Spanish Hash number on Widget and Dashboard
- If two hash numbers exist both should be visible
- Accessible to all users

