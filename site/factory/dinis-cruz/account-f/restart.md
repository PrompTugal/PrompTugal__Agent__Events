# cl-6.events: restart

If this session ends, a new one:
1. Clones PrompTugal/PrompTugal__Agent__Events (this home) and attaches PrompTugal/PrompTugal__News__Events with push, plus a read-only clone of PrompTugal__News__Website (dev, full history).
2. Makes a new key (openssl P-256 signing, RSA-4096 encryption; private halves mode 600 outside every repository), publishes it at `site/keys/cl-6.events.json` alone in its own commit, and marks the old one superseded. Asks the conductor to add it to the website's `board/keys.json`.
3. Sets ssh signing in each clone: gpg.format ssh, gpg.ssh.program ssh-keygen (install openssh-client if missing), user.signingkey, commit.gpgsign true. Trailers on every commit: Agent: cl-6.events@PrompTugal.dinis and Claude-Session: <its URL>.
4. Reads agent.json, now.md, learnings.md here, then history/PrompTugal__News__Events/board/team/events/debriefs/ and status.json, then the website's CLAUDE.md and board/guidance/README.md.
