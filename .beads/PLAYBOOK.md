# Beads setup for this repo (life-itself/research)

Prefix: `sorr` (Seeds Of Renaissance Research). Backend: Dolt, embedded mode.
Remote: `git+ssh://git@github.com/life-itself/research.git`

## Normal workflow

Start of session:
```bash
git pull
bd dolt pull
bd status
```

Work:
```bash
bd ready
bd create "Short issue title"
bd update sorr-xxxxxx --claim
bd close sorr-xxxxxx --reason "Implemented"
```

End of session:
```bash
bd dolt push
git add -A
git commit -m "..."
git push
```

## Hooks

bd-managed hooks live in `.beads/hooks/` and `core.hooksPath` is set to that
dir. They already run `bd hooks run <event>` which handles dolt pull/push
internally on post-merge / post-checkout / pre-push — no extra manual
wrapper scripts were needed on top for this bd version (1.1.2).

## Fresh clone on another machine

```bash
git clone git@github.com:life-itself/research.git
cd research
bd doctor      # not supported in embedded mode; use bd context/status instead
bd dolt remote list
bd dolt pull
bd status
```

If beads isn't initialized (missing `.beads/config.yaml`/`metadata.json` is
unlikely since these are tracked), run `bd bootstrap` then `bd dolt pull`.

## Troubleshooting

```bash
bd context
bd dolt remote list
bd dolt status
git status --short --branch
```

Then retry: `git pull`, `bd dolt pull`, `bd dolt push`. Do not delete
`.beads/`, remove the remote, or force-reinit as a first response.

See `~/src/rufuspollock/agent-skills/beads-sync-playbook.md` for the
general playbook this was set up from.
