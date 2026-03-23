# Atlas Integration

*This is a placeholder for Atlas data integration. When implemented, load
this file to query account data and pre-populate discovery findings.*

---

## Status: Not yet implemented

---

## Planned data sources

When Atlas integration is active, query these before discovery or demo planning
to avoid re-asking questions already answered.

### Customer record
- **Use case** and use case tier
- **Tech stack** via `technology` field
- **Enterprise trigger** via `reasonForEnterprise`
- **Company overview** via `companyOverview`
- **Org chart** via `orgChartDiagram`

### Meeting notes
- Prior discovery notes via `meetingNotes` for the account
- Raw notes and recordings via `rawNotes`, `meetingRecording`
- Use to pre-fill the discovery output template before the call

### Sanity project
- Linked project via `sanityProject`
- Current plan, usage signals, API volume
- Use to gauge actual engagement level vs. stated interest

### Technical check-ins
- Prior SE conversations via `techCheckInNotes`
- Use to understand what's already been discussed, demoed, or validated

---

## Planned workflow

1. SE provides account name or ID
2. Query Atlas for all sources above
3. Pre-populate the discovery output template with known data
4. Flag gaps — "I found X, Y, Z in Atlas. I still need to learn about [gaps]."
5. In demo plan mode, use Atlas data to skip redundant discovery and go
   straight to plan generation
