# Logic App

Current workflow: HTTP request trigger, JSON validation, points condition, and success/error response branches. The positive-points path returned HTTP 202 during testing.

**Service Bus publishing:** attempted through an HTTP action and SAS token after the managed connector connection was blocked by Azure Policy. Queue metrics showed zero incoming messages before the sandbox expired, so delivery remains unverified.

Add a sanitized workflow definition here. Remove signed callback URLs, keys, tokens, tenant IDs, and subscription-specific values before committing.
