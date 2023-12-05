---
title:  Notices Summary
---

import DashboardImg from '@site/static/images/ms-telex-ui/dashboard.png';

# Notices Summary

<img src={DashboardImg} />

### HIX
- [HIX-174237](../HIX/HIX-174237)
- [HIX-174248](../HIX/HIX-174248)

### Tasks

#### HIX-174237
Add both Spanish and English hash numbers to Dashboard and Widget.

#### HIX-174248
- “Triggered Notices” button only available for Management (clarification with Marc what is consider Management)
- “Delivered (last 7 days)”, “Waiting for release”, and “Errors” columns only available for Management
- Replace email address with name within “recipient” column of Triggered Notices.


### User Stories / Unit Tests
#### HIX-174237
- User should be able to view English and Spanish Hash number on Widget and Dashboard
- If two hash numbers exist both should be visible
- Accessible to all users

#### HIX-174248
- “Triggered Notices” button only available for Management
- “Delivered (last 7 days)”, “Waiting for release”, and “Errors” columns only available for Management
- Failed Table should contains recipient instead of email address




