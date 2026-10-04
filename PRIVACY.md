#Privacy Policy

**BallotTSR and the Election Secretary Web Portal**
Last updated: 4/10/2026

BallotTSR is a Reddit app that runs polls and elections for r/thespinroom. The Election Secretary Web Portal is a public website that publishes official election records. This policy explains what data is used and where it goes. If anything here is unclear, [contact us](https://www.reddit.com/u/PickleArtGeek).

## 1. What the app processes
- **Reddit username and eligibility data.** The app checks who may vote (for example account age, karma, or a voter ID where an election uses one) and prevents double voting.
- **Ballots.** Votes are stored while an election is open so they can be counted.
- **Election settings** configured by moderators.

The app does not collect email addresses, IP addresses, private messages, browsing history, or any private Reddit profile data.

## 2. Where data is stored
Ballots and eligibility records are stored in Reddit's Devvit platform storage and are not shared outside it, except as described in section 3.

## 3. What is sent outside Reddit
The app sends election results to a public GitHub repository, [Election Secretary Web Portal](https://github.com/pickleartgeek/ElSec), using the GitHub API at `api.github.com`. This is the only external service it contacts.

- **While an election is open:** aggregate tallies only (vote totals per candidate or option per (randomly assigned) voter group).
- **After an election closes:** final results and, where an election publishes them, an anonymized ballot-level file. Ballot files contain per-ballot and rankings or scores plus voter group. They contain no usernames or VoterIDs.

Published records are public and may be copied by anyone. Please read section 5 before voting.

## 4. What we do not do
We do not sell data, show ads, or build profiles. We do not share data with third parties other than publishing the results described above. We do not use Reddit data to train machine learning models.

## 5. Public records and retention
Election results are official public records and are kept permanently, including in the repository's version history. Because ballots are anonymized, a published ballot cannot be linked back to a person by us, and we generally cannot remove it. Eligibility and voter records in Devvit storage are deleted when the app is uninstalled.

## 6. Your choices
You can ask what voter data we hold about your account or ask us to delete it, using the contact above. If you delete your Reddit account, the app removes data linked to that username as Reddit's platform requires. Anonymized published results remain.

## 7. Children
Reddit requires users to be at least 13. The app does not knowingly process data of anyone under 13.

## 8. Changes
We may update this policy. The date at the top shows the latest version, and earlier versions stay available in the repository history.

This app is not affiliated with or endorsed by Reddit, Inc.
