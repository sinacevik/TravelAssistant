# TravelAssistant

> Portfolio mirror of the team project maintained at
> [Travel-Assistant-Project/TravelAssistant](https://github.com/Travel-Assistant-Project/TravelAssistant).
> The canonical repository is the source of truth for current code and setup instructions.

TravelAssistant is a team-built travel-planning application. Its React Native client communicates with an ASP.NET Core API that persists trip data in PostgreSQL and integrates with AI-assisted planning and external travel services.

## My contribution

I owned the first route-planning persistence slice in the .NET backend:

- implemented the `POST /api/routes/plan` endpoint
- connected the endpoint to the project's AI planning service
- added the `RoutePlan` EF Core entity and database mapping
- created the PostgreSQL migration for persisted route plans
- returned the generated trip plan after successful persistence

**Evidence:** [merged pull request #7](https://github.com/Travel-Assistant-Project/TravelAssistant/pull/7)

That pull request is the precise scope I claim as my individual contribution. Other features in the repository were developed collaboratively by the project team.

## Team project architecture

| Area | Technologies |
| --- | --- |
| Mobile client | React Native, Expo, TypeScript |
| Backend | C#, ASP.NET Core, Entity Framework Core, REST APIs |
| Data | PostgreSQL, Redis |
| Integrations | AI-assisted route planning, places, weather, and event services |
| Workflow | Git branches, pull requests, and code integration |

## What the contribution demonstrates

- designing and implementing an ASP.NET Core controller action
- mapping a request and service response into a persistent data model
- configuring EF Core entities and migrations
- working with PostgreSQL in a team-owned backend
- delivering a scoped feature through a reviewed and merged pull request

## Inspect or build the canonical project

```bash
git clone https://github.com/Travel-Assistant-Project/TravelAssistant.git
cd TravelAssistant
dotnet restore TravelAssistant.sln
dotnet build TravelAssistant.sln
```

Runtime configuration requires local environment values for the database and external services. Refer to the
[canonical repository](https://github.com/Travel-Assistant-Project/TravelAssistant) for the current configuration and application startup instructions. Never commit real credentials or API keys.

## Repository status

This user-owned repository is kept as a portfolio mirror. Issues and pull requests for the active team project should be opened in the [canonical repository](https://github.com/Travel-Assistant-Project/TravelAssistant).
