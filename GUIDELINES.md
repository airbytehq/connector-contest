# Guidelines for Airbyte Hacktoberfest

## Step 1
Check out the [issues page](https://github.com/airbytehq/hacktoberfest-2021/issues) and look for a connector that you're interested in building. If you can't find one that you want to do or if you have one already in mind that isn't here, simply create an issue for it!

## Step 2
Comment on the connector issue you're interested in with "I'll work on this one!" or something to that extent. It's first-come first-serve, so if someone has commented on it already, it's theirs to work on. If there is no activity within five days of someone commenting, we'll look to free up the issue again.

As a heads up, you can only be working on one connector at a time!

## Step 3
Once you have commented, we will respond telling you that you're good to go. You can now start working on your connector!

## Step 4

Create your connector in accordance with the following checklist:

In order for your connector to be eligible for rewards, you must pass the following criteria within the event's duration:

### Connector Checklist

- [ ] Grant edit access to maintainers ([instructions](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/allowing-changes-to-a-pull-request-branch-created-from-a-fork#enabling-repository-maintainer-permissions-on-existing-pull-requests))
- [ ] Secrets in the connector's spec are annotated with `airbyte_secret`
- [ ] Unit & integration tests added and passing. Community members, please provide proof of success locally e.g: screenshot or copy-paste unit, integration, and acceptance test output. To run acceptance tests for a Python connector, follow instructions in the README. For java connectors run `./gradlew :airbyte-integrations:connectors:<name>:integrationTest`.
- [ ] Code reviews completed
- [ ] Documentation updated
  - [ ] Connector's `README.md`
  - [ ] Connector's `bootstrap.md`. See [description and examples](https://docs.google.com/document/d/1ypdgmwmEHWv-TrO4_YOQ7pAJGVrMp5BOkEVh831N260/edit?usp=sharing)
  - [ ] `docs/SUMMARY.md`
  - [ ] `docs/integrations/<source or destination>/<name>.md` including changelog. See changelog [example](https://docs.airbyte.io/integrations/sources/stripe#changelog)
  - [ ] `docs/integrations/README.md`
  - [ ] `airbyte-integrations/builds.md`
- [ ] PR name follows [PR naming conventions](https://docs.airbyte.io/contributing-to-airbyte/updating-documentation#issues-and-pull-requests)
- [ ] Connector added to connector index like described [here](https://docs.airbyte.io/connector-development#publishing-a-connector)
   
## Step 5

Merge your PR and claim your reward! You can also now work on another connector if you're feeling inspired!