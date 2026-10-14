# Contributing to the Joltcrack Database

Welcome to the community joltcrack database. If you have been processing runs through Stick Studio or a custom tracker and have clean JSON output of the cracked session ticks, you can add it to this repository.

Having a centralized collection of jolt data makes it easier to verify anomalies, analyze server desyncs, and cross-reference splices without having to brute-force the PRNG seeds and phases from scratch for every run.

## How to Submit Your JSON

If you have a new jolt JSON to submit, please follow the standard PR workflow below:

1. **Fork the Repository**: Click the **Fork** button at the top right of this GitHub page to create your own copy of the database.
2. **Upload Your File**: Navigate to the `/cracks` folder in your fork and upload your JSON file.
* **Naming Convention:** Name the file clearly using the runner and the event name (e.g., `dream_5_hunters_finale_rematch.json` or `fineberg_manhunt.json`). Do not submit files generically named `data.json`.


3. **Verify Formatting**: Ensure your JSON contains the required, standard jolt data. It must include:
* The food level.
* The 10-shank visual vector pattern (e.g., `17 ++0+--0--0`).
* The cracked session uptime/ticks.
* The corresponding video timestamps.


4. **Open a Pull Request**: Go to the "Pull Requests" tab on this main repository, click **New pull request**, and compare the changes across your fork to submit it.

### What to Include in the PR Description

When creating your PR, please include the following details in the description box:

* A direct link to the original YouTube or Twitch VOD that the data was tracked from.
* A brief summary of the results: note whether the run was continuous (a clean 1:1 slope of video time to game ticks) or if you found any clear splice anomalies, such as vertical tick jumps or locked animation phases across cuts.

PRs will be reviewed and merged into the main branch as they are submitted.
