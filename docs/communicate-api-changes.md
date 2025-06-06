# Communicating API Changes

- **Status:** Unknown

!!! tip "Nexus Mods should communicate breaking API changes and updates to the outside world"

    When we introduce breaking changes or API updates, Modding Tool authors dependent
    on our APIs need to be notified.

This is so they can:

- Fix issues before users blame them for problems outside their control.
- Add new functionality that takes advantage of newer site features.

## The Problem

!!! warning "We sometimes make breaking changes without proper notification to dependent tools"

As a Mod Framework author, a certain website I have experience with (***NOT named Nexus Mods***) has,
in the past made breaking changes. Not often, usually not intentionally, but it happened enough times
to be notable; and that has me very wary of these things.

That's why I want to talk about the problem.

### Communication Issues

!!! info "Breaking changes are only ever mentioned in our `api-change-discussion` channel on Slack"

    Sometimes, in rare occasions, changes slip by and are not brought up there.

This has, for example, led to a situation where ***our internal App team*** has once ran across a breaking
change that was not mentioned anywhere. This could have gone bad, especially if the change went live
right around the same time as the App release, and we can't fix it in time.

Equally as importantly, authors of external modding tools who depend on our APIs are never informed
of any sort of changes whatsoever.

### User Behavior Challenges

!!! info "End users are not very receptive to reporting these sorts of issues nowadays"

- **Wait-and-see attitude**: Users are conditioned to just 'wait' until something's fixed
- **Delayed reporting**: As a Mod Tool author, I'd only often get to hear about it 2-3 days later due to that
- **Blame attribution**: Tool authors receive bad reputation for what's not their fault

!!! example "Real impact"

    Some users don't like to update (see Vortex version stats in telemetry, as an example).  
    As a Mod Tool author, you sometimes receive a bad reputation for what's not your fault.

### The Core Issue

1. If changes are not communicated, we don't test against them.
2. If we don't test against them, issues cannot be caught early.
3. If issues are not caught early, they are passed to the end user, and can't be fixed in a timely manner.
4. In the end, users may experience issues for days at a time.

## What's Needed

!!! tip "Simple solutions that would prevent most issues"

I'm not one to give 'magic bullets', but at least the following basic things could help.

- **Public API change notifications**: Announce breaking changes to tool authors publicly, not just in internal channels
- **Advance notice**: Give mod tool authors time to prepare for changes
- **A Changelog**: Can we add a changelog to [graphql.nexusmods.com](https://graphql.nexusmods.com)?
