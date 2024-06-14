# Database Storage

## Status

Proposed

## Context

The application needs to store and retrieve data, but a decision has been made not to use a database.

## Decision

We propose to use local storage for persisting data. React Native provides an AsyncStorage module that can be used for this purpose.

## Consequences

Using local storage will simplify our architecture and eliminate the need to manage a separate database system. However, it may limit the amount of data we can store and we will need to manage data serialization and deserialization ourselves.