# Description
Public Repository for showing problems of turborepo pruning a monorepo with bun lockfiles.

# Issue
Included are already 2 output folders that were pruned from the codebase, without any changes inbetween. If the two bun lockfiles from out/json/bun.lock and out2/json/bun.lock get both put into a diffchecker it shows that the optionalPeers just get reordered in the file.

# Reproducibility
I added 2 scripts into the root package.json: prune and prune-second.
prune generates the first prune to the folder out and prune-second generates the second folder to out2 in the root directory.
