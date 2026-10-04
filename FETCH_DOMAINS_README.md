## Fetch Domains

This app requests one external domain.

### `api.github.com`

**Why it is needed.** Elections run by this app are published as official public records on the Election Secretary Web Portal, which is hosted from a public GitHub repository ([REPO URL]). Devvit's built-in capabilities (Redis and the Reddit API) cannot write to an independent public repository, so the app uses the GitHub contents API to publish results.

**What is sent.**
- While an election is open: aggregate vote tallies as `results.json`, updated on a schedule (no more often than every [N] minutes).
- After an election closes: the final results and, where the election publishes them, an anonymized ballot-level file.

No usernames, IP addresses, or private Reddit data are included in any request.

**How it works.** A scheduler job reads tallies from Redis and writes files with WIP. The repository token is stored as an app setting (secret) and is never exposed to client code. Requests use HTTPS and are made from server-side code only.

**Policies.** [Privacy Policy](PRIVACY.md) and [Terms of Service](TERMS.md).

`devvit.json`:

```json
"http": {
  "domains": ["api.github.com"]
}
```
