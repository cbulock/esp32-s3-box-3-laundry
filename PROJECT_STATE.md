Laundry Screen MVP

Status
- Laundry UI page added with washer/dryer status, remaining time, and user selection.
- Uses Home Assistant entities for machine state, job state, completion time, and user input_selects.
- Screen refreshes every 5s while the laundry page is active.

Assumptions
- Completion time sensors are numeric UNIX timestamps (seconds).
- Machine/job state sensors expose string states like running/idle/out-of-order.

Next steps
- Confirm actual HA state strings and adjust mapping for running/available/out-of-order.
- If completion_time is not numeric, add parsing or swap to a numeric template sensor in HA.
- Add a dedicated laundry page icon or quick navigation shortcut if desired.
