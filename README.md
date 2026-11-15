# Denis Andreyev

Backend developer in Astana, Kazakhstan, and a CS student at Nazarbayev University (class of 2027).
I build and run production systems on my own and send fixes to open-source C, C++ and Julia projects.
Open to backend, DevOps and full-stack roles, remote or in Astana.

[LinkedIn](https://www.linkedin.com/in/denisxandreyev/) · [denisxandreyev@gmail.com](mailto:denisxandreyev@gmail.com)

## In production

- **[Happy End](case-studies/happyend.md)**: e-commerce for three city sites, ~7,000 monthly users. Next.js, a PHP API and PostgreSQL. I moved the live store off 1C-Bitrix in September 2026 without losing orders, and a bank callback only counts once the bank's status API confirms the payment and the amount.
- **[City news platform](case-studies/city-portals.md)**: a Go and PostgreSQL platform behind two regional news portals. Row-level security keeps each portal's content rows apart, and full-text, trigram and vector search run in the same database.
- **[MusicRoomBot](https://github.com/unsound-mint/MusicRoomBot)**: Telegram booking bot used by ~200 NU students since December 2025. A unique constraint stops double booking and an advisory lock stops one user from going over the weekly limit. Both races are tested against PostgreSQL in CI.

## Merged upstream

- MangoHud: [apply `gl_vsync` to EGL per surface](https://github.com/flightlessmango/MangoHud/pull/2187), [start logging when the HUD is hidden](https://github.com/flightlessmango/MangoHud/pull/2189), [keep running when a hwmon sensor can't be read](https://github.com/flightlessmango/MangoHud/pull/2190)
- DNF5: [`reposync --latest-limit=N`](https://github.com/rpm-software-management/dnf5/pull/3008)
- GPUArrays.jl: [range indexing kernels](https://github.com/JuliaGPU/GPUArrays.jl/pull/839), [`@fastmath` reductions](https://github.com/JuliaGPU/GPUArrays.jl/pull/840)
- FITSIO.jl: [full COMMENT/HISTORY cards](https://github.com/JuliaAstro/FITSIO.jl/pull/246), [CONTINUE cards written as they are](https://github.com/JuliaAstro/FITSIO.jl/pull/247)

In review: [ROCm FP8 conversions](https://github.com/ROCm/rocm-systems/pull/14307), [CARTA save through a symlink](https://github.com/CARTAvis/carta-backend/pull/1648), [uutils `date` time zones](https://github.com/uutils/coreutils/pull/16148), [libsolv glob file search, 19× faster](https://github.com/openSUSE/libsolv/pull/643).

## Projects

- **[payhook](https://github.com/unsound-mint/payhook)**: Go payments and webhooks service. A status change and its outbox row commit in one transaction, callbacks go out through NATS JetStream, and the retry limit is counted in PostgreSQL. Helm chart and a kind rolling-restart test.
- **[payhook-infra](https://github.com/unsound-mint/payhook-infra)**: Terraform for payhook on AWS, with the requirements written as `terraform test` checks and keyless GitHub OIDC deploys. Not applied to a live account yet.
- **[Parenting Planner](https://github.com/unsound-mint/parenting-planner)**: a weekly plan for each parent, built from the family's own records and cited health guidelines. Made at Business Cup 2.0 with a team of three. Go API, PostgreSQL, Next.js, an OpenAPI contract with generated clients and a rules engine of pure functions. [Live demo](https://parenting.unsoundmint.com).
- **[CQA](https://github.com/unsound-mint/cqa-hackathon)**: scoring of support conversations, 4th of 250 teams at the CQA Hackathon. Model output is checked against the transcript before it counts, and totals are computed in code.
- **[Vesqira](https://github.com/unsound-mint/vesqira)**: research workspace for astronomical data cubes, with a Go control plane, Python workers and Slurm jobs. Pre-release.

Research code: [VGT.jl](https://github.com/ISM-NU/VGT.jl) and [ROHSA-LMC](https://github.com/ISM-NU/ROHSA-LMC) for the [ISM-NU](https://github.com/ISM-NU) group's work on magnetic fields in the Large Magellanic Cloud, [nuclear-morphometry](https://github.com/unsound-mint/nuclear-morphometry) (GPU microscopy pipeline), [vbench](https://github.com/unsound-mint/vbench) (energy use of fine-tuning on a laptop GPU).
