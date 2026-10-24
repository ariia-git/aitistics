# Archive workflow

Use this guide when adding or managing demonstration files, whether working manually or with an agent.

## Add a run

1. Create `runs/<system>/<number>-<run-name>/` using lowercase kebab-case. Each system has its own numbering sequence; add a system directory only when it has a run.
2. Adapt the [run README](../templates/run-readme.md) and [metadata](../templates/metadata.yaml) templates.
3. Place original generation settings under the run's `config/` directory and representative frames under `images/`. Preserve source filenames and contents unless privacy requires sanitisation.
4. Record the published YouTube URL and supported generation details. Use portable relative paths for repository files; leave unknown values blank.
5. Add the run and a brief description to the root README and the system catalogue.

## Before publishing

- Check that Markdown links and metadata file references resolve.
- Review text and configuration for secrets, personal information, and private machine paths. Document any necessary sanitisation without exposing the original sensitive values.
- Keep completed video renders outside Git. Images are ordinary Git files; do not use Git LFS or transform source frames.
- Review the intended changes, commit through the existing repository, and push without rewriting history or discarding unrelated work.

See the [methodology](methodology.md) for documentation principles.
