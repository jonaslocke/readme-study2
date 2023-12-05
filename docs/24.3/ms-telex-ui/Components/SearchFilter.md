---
title:  Search Filter
---

import SearchFilterImg from '@site/static/images/ms-telex-ui/search-filter.png';

# Search Filter

<img src={SearchFilterImg} />

### HIX
- [HIX-174250](../HIX/HIX-174250)

### Tasks
- Add "clear" button to reset all values.
	- Clears “saved filters” and “advanced search”
- Add "Save" button, 
	- Expose “Save” Button if saved filter is selected and advanced search criteria is change.
	- Allowing admin to edit existing saved filter.
	- If rule is currently active, disable the save button.
	- If disabled, show tooltip on hover.
	- Tooltip label says, "Disable rule to make changes to this filter."
	- This button should only be enabled if filter is not currently active.
	- Modified Rename button function.
	- Do not display unless saved filter is selected or value in “advance search” field.


### User Stories / Unit Tests
- Search Filter Component should display clear and save buttons
- Clear button should clear saved filter selections and advanced search field
- Save button should only be expose if saved filter is selected and advance search criteria is changed
- Tooltip should be display on hover if save button is disabled
- Save button should be disabled if advance search is empty or saved filter is not selected
- Rename is only display if saved filters is selected