# Conflux build of Graphiti

This branch is Graphiti `v0.30.2` plus one fix, packaged as `0.30.2+conflux.6`.

- Fix: `remove_episode` keeps facts that other episodes still support, removes the
  episode from surviving facts, and rebuilds surviving entity summaries from the
  remaining episodes. Branch `fix/remove-episode-shared-support`, proposed upstream
  for getzep/graphiti#1837.

Nothing else differs from upstream `v0.30.2`. Build the wheel with `uv build --wheel`.
