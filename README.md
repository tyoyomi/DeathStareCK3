# Death Stare

Crusader Kings III character-interaction mod. Version 0.1.0. Supported game version 1.20.*.

Death Stare a vassal (or realm target) to briefly cow them into Yes Man behavior toward you. While cowed, curated vanilla asks (conversion, marriage, call ally, join war, negotiate alliance, offer vassalization) auto-accept without spending gold or hooks. Optional force-government verb for eligible tribal/clan/feudal liege-convert cases.

Canonical working copy: `Documents/Development/CK3 Mods/ds`.

Soft peers: Supreme Sovereign, Exalted Advisor, Succession Unity (detection only; no hard dependency).

## Vanilla footprint (LIOS)

Full interaction redefines:

- `demand_conversion_interaction`
- `demand_conversion_vassal_ruler_interaction`
- `ask_for_conversion_interaction`
- `ask_for_conversion_courtier_interaction`
- `call_ally_interaction`
- `negotiate_alliance_interaction`
- `join_war_interaction`
- `offer_vassalization_interaction`

Shared packs / triggers:

- `religion_demand_conversion_default_modifier`
- `offer_vassalization_interaction_ai_acceptance_general`
- `negotiate_alliance_interaction_ai_acceptance`
- `marriage_ai_accept_modifier`
- `marriage_interaction_auto_accept_trigger`

Decisions (AI nudge):

- `convert_to_feudalism_liege_converted_decision`
- `convert_clan_to_feudalism_through_liege_decision`
- `convert_feudalism_to_clan_through_liege_decision`

Load Death Stare after other mods that also redefine these keys if DS must win.
