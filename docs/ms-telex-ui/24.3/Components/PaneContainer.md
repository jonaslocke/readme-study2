---
title:  Pane Container
---

import PaneContainerImg from '@site/static/images/ms-telex-ui/pane-container.png';

# Pane Container

<img src={PaneContainerImg} />

### HIX
- [HIX-174250](../HIX/HIX-174250)

### Tasks
- Prevent same test case from being uploaded multiple times.
	- When a new test case is uploaded or saved, check json against existing saved test cases. Throw error if existing test case already exists and include the name of the existing json.

### User Stories / Unit Tests
- User should not be able to save existing test case name
- Error message should display if test case name already exists