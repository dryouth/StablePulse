# StablePulse

Canonical prompt backup for the StablePulse weekly report workflow.

## Active version

**v13.3.1** is the only active weekly report prompt set.

- Step 0: context loader
- Step 2: Korean report generator
- Step 5: editorial QA and revision
- Step 2E remains optional and is not part of the weekly automatic bundle.

## Technical source routing

Section 7 technical analysis uses the completed-candle TradingView source routed through S5/S6.

- Active Cycle Peak/Trough and all technical cycle anchors come only from S5/S6 `CYCLE_ANCHORS`.
- S4 `ETH_Cycle` Peak/MDD is RRI cycle-duration and drawdown context only.
- S4 `ETH_Cycle` and S5/S6 `CYCLE_ANCHORS` must not be compared to generate a conflict or review warning.
- Differences between those source classes are `EXPECTED_SOURCE_TIME_DIFFERENCE`.

## Integrity

Verify all files against [MANIFEST.sha256](MANIFEST.sha256). Do not use a prompt whose SHA-256 does not match the manifest.
