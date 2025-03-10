# Changelog

## Unreleased

* Update OTel API version to `1.3.2`.
  ([#917](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/pull/917))

## 1.0.0-rc9.7

Released 2022-Jul-25

* Update the `ActivitySource` name used to the assembly name: `OpenTelemetry.Instrumentation.StackExchangeRedis`.
([#485](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/pull/485))
* Drain thread is marked as background. It allows to close the application
  even if the instrumentation is not disposed.
([#528](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/pull/528))

## 1.0.0-rc9.6

Released 2022-Jun-29

* Added the EnrichActivityWithTimingEvents option to
  StackExchangeRedisCallsInstrumentationOptions to be able to disable adding
  ActivityEvents (Enqueued, Sent, ResponseReceived) for Redis commands to
  Activities since there is no way to clear these after they have been added.
  This defaults to true to maintain current functionality.

## 1.0.0-rc9.5 (source code moved to contrib repo)

Released 2022-Jun-06

* From this version onwards, the source code for this package would be hosted in
  the
  [contrib](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/tree/main/src/OpenTelemetry.Instrumentation.StackExchangeRedis)
  repo. The source code for this package before this version was hosted on the
  [main](https://github.com/open-telemetry/opentelemetry-dotnet/tree/core-1.3.0/src/OpenTelemetry.Instrumentation.StackExchangeRedis)
  repo.

## 1.0.0-rc9.4

Released 2022-Jun-03

## 1.0.0-rc9.3

Released 2022-Apr-15

* Removes .NET Framework 4.6.1. The minimum .NET Framework version supported is
  .NET 4.6.2.
  ([#3190](https://github.com/open-telemetry/opentelemetry-dotnet/issues/3190))

* Bumped minimum required version of `Microsoft.Extensions.Options` to 3.1.0.
  ([#2582](https://github.com/open-telemetry/opentelemetry-dotnet/pull/3196))

## 1.0.0-rc9.2

Released 2022-Apr-12

## 1.0.0-rc9.1

Released 2022-Mar-30

## 1.0.0-rc10 (broken. use 1.0.0-rc9.1 and newer)

Released 2022-Mar-04

## 1.0.0-rc9

Released 2022-Feb-02

## 1.0.0-rc8

Released 2021-Oct-08

* Adds SetVerboseDatabaseStatements option to allow setting more detailed
  database statement tag values.
* Adds Enrich option to allow enriching activities from the source profiled
  command objects.
* Removes upper constraint for Microsoft.Extensions.Options dependency.
  ([#2179](https://github.com/open-telemetry/opentelemetry-dotnet/pull/2179))

## 1.0.0-rc7

Released 2021-Jul-12

## 1.0.0-rc6

Released 2021-Jun-25

* `AddRedisInstrumentation` extension will now resolve `IConnectionMultiplexer`
  & `StackExchangeRedisCallsInstrumentationOptions` through DI when
  OpenTelemetry.Extensions.Hosting is in use.
  ([#2110](https://github.com/open-telemetry/opentelemetry-dotnet/pull/2110))

## 1.0.0-rc5

Released 2021-Jun-09

## 1.0.0-rc4

Released 2021-Apr-23

* Activities are now created with the `db.system` attribute set for usage during
  sampling.
  ([#1984](https://github.com/open-telemetry/opentelemetry-dotnet/pull/1984))

## 1.0.0-rc3

Released 2021-Mar-19

## 1.0.0-rc2

Released 2021-Jan-29

## 1.0.0-rc1.1

Released 2020-Nov-17

## 0.8.0-beta.1

Released 2020-Nov-5

## 0.7.0-beta.1

Released 2020-Oct-16

* Span Status is populated as per new spec
  ([#1313](https://github.com/open-telemetry/opentelemetry-dotnet/pull/1313))

## 0.6.0-beta.1

Released 2020-Sep-15

## 0.5.0-beta.2

Released 2020-08-28

## 0.4.0-beta.2

Released 2020-07-24

* First beta release

## 0.3.0-beta

Released 2020-07-23

* Initial release
