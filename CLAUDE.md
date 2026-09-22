# Modulark Lighting — Context for all sessions

Modulark Tech Labs Pvt Ltd (India). Room-level ambient lighting system.
A sensing brain solves for how a room should look and commands wireless
light modules to reach it. Closed loop. No app, no account, no internet.

**Read `docs/00-DECISIONS.md` before doing any work in this repo.** It is
the locked-decision log. Do not re-litigate decisions marked LOCKED without
an explicit instruction from the founder.

## Non-negotiable engineering rules (compliance-driven)

These exist to keep the product certifiable under BIS CRS. Violating any of
them invalidates the certification path and costs ~3 months.
See `docs/02-COMPLIANCE.md` for the reasoning.

1. **No mains voltage inside any Modulark enclosure.** Mains terminates
   inside a BIS-registered, fully encapsulated AC-DC module. Everything
   downstream is SELV DC (<=50 V).
2. **No uncertified plastic in the fire-risk path.** Enclosures are CNC
   aluminium. The PCB mounts to metal via metal standoffs. There is no
   internal plastic structural frame.
3. **Diffusers are bought, not printed.** Must be PC with supplier
   GWIT/GWFI material data on file.
4. **No 3D-printed part ships in a certified product.** Printing is for
   prototyping and fixtures only.
5. **Cells are bought BIS-registered (IS 16046).** Modulark does not
   register cells itself.
6. **The Pack has no USB host output.** It is a battery for a luminaire,
   not a portable charger. Adding an output port re-triggers IS 13252.

## Current phase

Pre-revenue. v1 scope is three SKUs: Core, Field, Pack. BIS CRS on the
Field module is the critical path and gates all revenue.

## Repo conventions

- Work on the branch you are assigned. Do not push to other branches.
- Rolled-up product and kit costs live only in
  `docs/04-UNIT-ECONOMICS.md`. Component-level costs live only in
  `docs/06-BOM-FIELD-MODULE.md`. Do not duplicate either; link instead.
- Anything unverified is tagged `[CONFIRM]`. Do not strip the tag without
  citing a primary source.
