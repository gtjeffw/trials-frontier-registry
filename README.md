# Trials Frontier community registry

A list of published Trials Frontier ghost bundles: other riders' best times and ghost replays, made and published
with trials-frontier-patch (`scripts/ghost_bundle.py`; not public yet). Its `scripts/community.py` reads
[`registry.json`](registry.json) to bring every listed rider into your game.

**Getting listed.** Open an issue here titled `bundle: <owner>/<repo>` ("Add a ghost bundle"); once
trials-frontier-patch is public, `ghost_bundle.py publish` and `update` will offer to open it for you. For now
requests are checked by hand; then a GitHub Action ([`automation/registry.yml`](automation/registry.yml), switched
on at that point) will check each request at once and reply, and every night find new bundles by their GitHub topic
(`trials-frontier-bundle`) and re-check the listed ones. A bundle is listed only if it is valid and every commit was
made through GitHub by the publisher the bundle names (GitHub signs those commits).

**What the list is, and is not.** Each entry names a repository, its publisher, rider, licence and the commit that
was checked. The registry only points to bundles: `community.py` still downloads and checks every bundle itself, so
a listing cannot vouch for data the registry does not hold. A bundle that stops passing the checks stays listed as
`failing` until it passes again.

The list itself is CC0 (public domain). Each bundle keeps the licence its publisher chose.
