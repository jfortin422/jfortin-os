# JavaScript Standards

## General

- Use a single namespace per solution.
- Avoid jQuery where native APIs exist.

## Dataverse

- Use formContext, never Xrm.Page.
- do not pass formContext from function to function, always pass the executionContext, unless coming from the ribbon, where only the formContext is supplied
- Minimize Web API calls.
- Have all fetchxml conditions or link entities on single lines
- comments in fetchxml are welcome to say which optionset values are selected 

## Power Pages

- Use delegated event handlers.
- Avoid duplicate validators.
- All custom validation messages must be localizable.
- Avoid unregistering handlers

## Error Handling

- Never swallow exceptions.
- Log all exceptions to tracing.
- Show user-friendly messages.

## Security

- Never expose secrets.
- Sanitize all HTML.
- Validate file names and extensions.

## Performance

- Avoid repeated DOM queries.
- Cache selectors.
- Avoid unnecessary Dataverse reads.