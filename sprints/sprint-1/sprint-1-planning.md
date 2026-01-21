# Sprint 1 Planning Session

Date: 14 Jan 2026
Sprint Goal: Allow employees to successfully book and manage conference rooms without conflicts.

## Attendees
- Product Owner: Stakeholder
- Scrum Master: Team lead
- Development Team: full-stack developers

## Velocity Target
20 story points

## Selected User Stories
| Story # | Title | Story Points |
|--------:|-------|--------------|
| 1 | Basic room booking | 8 |
| 3 | Room capacity filtering | 3 |
| 4 | Booking cancellation | 2 |
| 6 | Admin dashboard viewing | 5 |
| 8 | Visitor booking assistance | 2 |

## Dependencies
- Story #3 depends on room data model from Story #1
- Story #4 depends on booking creation (Story #1)
- Story #6 depends on booking data availability (Story #1 & Story #8)

## Risks
| Risk | Probability | Impact | Mitigation |
|-----|------------|--------|------------|
| API delays | Medium | High | Prioritise backend endpoints early |
| UI integration issues | Low | Medium | Early frontend-backend sync |

## Standup Cadence
Time: Daily at 09:00
Format: Yesterday / Today / Blocker