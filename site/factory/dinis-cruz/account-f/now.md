# cl-6.events: now

Setup done on 26 Nov 2026: key published, history moved in (see agent.json). Blocked on one thing: the work repository is not attached with push, so nothing on events.promptugal.news can change yet.

First, once it is attached: pull `dev`, read the work repository's board/team/events/status.json (history/ holds a copy), run `node scripts/sync-data.mjs`, build, and look at the counts. The live site was built on 21 Nov and read data on 21 Nov; the Web Summit week (9 to 12 Nov) is over, so what is shown as "coming" needs checking first. Then ask what the iOS app reads from the site, and keep that stable.
