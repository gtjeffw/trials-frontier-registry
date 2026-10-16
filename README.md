# Trials Frontier community registry

A list of published Trials Frontier ghost bundles: other riders' best times and ghost replays, made and published
with [trials-frontier-patch](https://github.com/gtjeffw/trials-frontier-patch) (`scripts/ghost_bundle.py`).
`scripts/community.py` in that project reads [`registry.json`](registry.json) to bring every listed rider into
your game.

**Getting listed.** `ghost_bundle.py publish` (and `update`) offers to open an issue here, titled
`bundle: <owner>/<repo>`; you can also open one yourself ("Add a ghost bundle"). A GitHub Action checks the bundle
at once and replies: it must be valid and every commit must have been made through GitHub by the publisher the
bundle names (GitHub signs those commits). Every night the Action also finds new bundles by their GitHub topic
(`trials-frontier-bundle`) and re-checks the listed ones.

**What the list is, and is not.** Each entry names a repository, its publisher, rider, licence and the commit that
was checked. The registry only points to bundles: `community.py` still downloads and checks every bundle itself, so
a listing cannot vouch for data the registry does not hold. A bundle that stops passing the checks stays listed as
`failing` until it passes again.

The list itself is CC0 (public domain). Each bundle keeps the licence its publisher chose.
