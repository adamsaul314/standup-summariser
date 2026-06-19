# standup-flow

This workflow receives raw standup notes from the user, runs blocker detection on the notes, passes the blocker result to the standup summariser, and returns a formatted standup summary.

## Workflow

1. Receive raw notes from the user.
2. Call the Blocker Detector agent with the raw notes.
3. Capture the blocker result.
4. Call the Standup Summariser agent with the raw notes and the blocker result.
5. Return the formatted standup summary to the user.

## Details

- Input: raw standup notes provided by the user.
- Blocker detection: determine whether the notes include an active blocker or impediment.
- Summarisation: produce a concise summary of what was done, what is next, and any blockers.
- Output: a structured standup summary, including the blocker result if applicable.

## Example flow

- User submits note: "Finished the API endpoint, waiting on design feedback before integration. Next I will update tests."
- Blocker Detector returns: "Waiting on design feedback before continuing integration."
- Standup Summariser returns:
  - What was done: Finished the API endpoint.
  - What is next: Update tests and integrate once design feedback arrives.
  - Blockers: Waiting on design feedback before continuing integration.
