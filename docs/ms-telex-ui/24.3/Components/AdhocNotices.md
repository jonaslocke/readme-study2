---
title:  Adhoc Notices Component
---

import AdhocImg from '@site/static/images/ms-telex-ui/adhoc-notices.png';

# Ad Hoc Notices

<img src={AdhocImg} /> 

### HIX
- [HIX-174244](../HIX/HIX-174244)


### Tasks
- Add brokers, assisters, and issuers to “Recipient Type” list on Adhoc Notices Component
- List should be in alphabetical order.
- Default value should be “consumers.”
- If any value is selected beside “consumers”, userId column (instead of householdId column) will be required in csv.

### User Stories / Unit Tests
- Brokers, assisters, and issuers should be presented in Adhoc Notices list and should be in alphabetical order.
- Default value should be “consumers.”
- If consumers is not selected, Note label should be update to say “userId column must be present(case-sensitive).”



