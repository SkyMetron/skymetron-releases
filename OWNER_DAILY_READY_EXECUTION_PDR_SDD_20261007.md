# PDR + SDD — skymetron-releases

**Authority:** https://github.com/SkyMetron/SkyGerSDDProjects/blob/vnext5-w0-canonical-resync/OWNER_DAILY_READY_PDR_SDD_EXECUTION_MASTER_20261007.md
**Class:** RELEASE ARTIFACTS
**Status:** draft specification only, no production feature created.

## PDR
Definir gate de distribuição Windows com integridade/rollback, sem publicar artefatos não aprovados.

## SDD / architectural role
Este repo é somente registro de releases e artefatos, sem fonte executável do produto. Definir contrato manifest SHA256, SBOM, release channel, versão, assinatura quando disponível, artefatos NSIS/portable, rollback. Não publicar release nem introduzir binários via esta PR; release deve vir de build validado localmente.

## Multi-agent
Responsible AGENT-H; AGENT-G independent reviewer; AGENT-A contract alignment. No agent shares mutable worktree. Evidence pass only after actual tests.

## Exit condition
Em build canário, pacote é instalável/atualizável/rollback e hash/SBOM correspondem; publishing gate owner-only; repo permanece artifact-only.

## Test plan
Release manifest schema, checksum validation with synthetic fixture, installer windows smoke, upgrade/rollback, malware/secret scan.

## Operational rule
Do not merge/release/deploy/archive/scrub without separate Owner approval. This PR may be updated with verified work and audit evidence. Freeze unrelated product sources and preserve historical release/secret artifacts. Report HEAD, build/test/security outcomes, recovery and blockers.
