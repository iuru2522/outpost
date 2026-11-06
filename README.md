# Outpost

ASP.NET Core Web API on .NET 10 LTS.

## Requirements

.NET SDK 10. The version is pinned in `global.json`.

## Run

```powershell
dotnet run --project src/Outpost.Api
```

The HTTPS profile listens on `https://localhost:7236` and `http://localhost:5197`.

## Endpoints

| Method | Path | Notes |
| --- | --- | --- |
| GET | `/weatherforecast` | Sample forecast from the Web API template |
| GET | `/openapi/v1.json` | OpenAPI document, Development only |

## Build

```powershell
dotnet build Outpost.slnx --configuration Release
```

## CI

GitHub Actions builds `Outpost.slnx` in Release on every push to `main` and on every pull request. The workflow is `.github/workflows/ci.yml`.
