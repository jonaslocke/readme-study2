---
title:  Widget
---

import WidgetImg from '@site/static/images/ms-telex-ui/widget.png';

# Widget

<img src={WidgetImg} />

### HIX
- [HIX-174237](../HIX/HIX-174237)
- [HIX-174239](../HIX/HIX-174237)

### Tasks

#### HIX-174237
- Add both Spanish and English hash numbers to Dashboard and Widget.

#### HIX-174239
- Moved Promote, Show Change, Edit from the Widget to top of Full Summary Top Nav bar
- Add tooltip to Import button (on Widget) and disable it if incomplete template exists.
- Tooltip should say, “Please delete incomplete template first” (subject to change)
- Change “Show Change" button should be "Show Changes".

### User Stories / Unit Tests

#### HIX-174237
- User should be able to view English and Spanish Hash number on Widget and Dashboard
- If two hash numbers exist both should be visible
- Accessible to all users

#### HIX-174239
- Update unit testing involving Promote, Show Change, and Edit button.
- Import button should display tooltip if incomplete exist, vice versa.
	- It should say, “Please delete incomplete template first” (subject to change)
