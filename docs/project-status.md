# SkyPoints project status

**Last updated:** 11 November 2026

## Completed / exercised
- Local project workspace created.
- Logic App (Consumption / multi-tenant) deployed in the KodeKloud sandbox.
- HTTP request trigger configured.
- JSON validation and points condition configured.
- Positive and negative points paths tested; positive path returned HTTP 202.
- Service Bus namespace and `aj-points-events` queue created.
- Dedicated SAS send policy created.
- Service Bus REST send attempt made from a Logic App HTTP action.

## Not verified / blocked
- Service Bus queue delivery was not verified. At sandbox expiry, the queue overview showed zero active messages and zero incoming messages.
- The Service Bus managed connector connection was blocked by `RequestDisallowedByPolicy`.
- APIM deployment was blocked by sandbox Azure Policy.
- No Function, database, Key Vault, managed identity, monitoring, ADF, or IaC implementation yet.

## Next session
1. Recreate or start a fresh sandbox.
2. Verify the Logic App HTTP action's exact response status and body.
3. Confirm one message appears in `aj-points-events` using Service Bus Explorer.
4. Only after confirming delivery, begin the Service Bus-triggered Function.
