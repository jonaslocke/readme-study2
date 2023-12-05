---
title:  Failed Table
---

import FailedTableImg from '@site/static/images/ms-telex-ui/failed-table.png';

# Failed Table

<img src={FailedTableImg} />

### HIX
- [HIX-174239](../HIX/HIX-174239)
- [HIX-174248](../HIX/HIX-174248)
- [HIX-174250](../HIX/HIX-174250)


### Tasks

#### HIX-174239
- Increased clarity on whether a failed notice when already retriggered. 
- On click of “retrigger notice” button, refresh list on left side.  Expectation is that: 
- Retriggered notice will automatically disappear. 
- Any updates (updated status, new records, etc) to list will automatically appear. 
- Additionally, every 3 seconds, auto-refresh list. 

#### HIX-174248
-	Replace email address with name within “recipient” column of Triggered Notices.
-	Wildcard search (check if this is doable client side)

#### HIX-174250
- Add Actions column in test case sample table
	- Within the column, include two buttons
		- Rename button – should allow user to rename the test case
		- Delete button – should allow user to delete test case

### User Stories / Unit Tests
- Brokers, assisters, and issuers should be presented in Adhoc Notices list and should be in alphabetical order.
- Default value should be “consumers.”
- If consumers is not selected, Note label should be update to say “userId column must be present(case-sensitive).”