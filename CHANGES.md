 * #365 - _Serilog.Sinks.ApplicationInsights_ now targets the new Azure Portal-based version (preview)
 * #367 - _Serilog.Sinks.MongoDB_ now targets the new preview driver (preview)
 * #369 - Fixed log message property in .NET 4.0 build of Elasticsearch sink

1.4.139
 * #125 - Merged _MonoTouch_ and _MonoAndroid_ sinks (**not currently published  to NuGet**)
 * #362 - Update Loggly sink package dependencies
 * #203 - _Azure Document DB_ sink

1.4.126
 * #354 - Added _Serilog.Extras.FSharp_

1.4.118
 * #351 - Azure Event Hubs sink

1.4.113
 * #329 - Write event properties as columns using the new `WriteTo.AzureTableStorageWithProperties()`
 * #346 - Pass all properties through to _Serilog.Sinks.NLog_ as context properties
 * #347 - Update _Serilog.Sinks.SignalR_ to SignalR version 2.1.0 (breaking)

1.4.99
 * #342 - Accept `ILogEventEnricher` rather than just `PropertyEnricher` to `ForContext`
 * #341 - Selectable logging level for request details in _Serilog.Extras.Web_

1.4.92
 * #340 - Accept an `Encoding` parameter on the file sinks
 * #336 - Use stream when writing to Splunk via HTTP
 * #335 - Remove use of `dynamic` when destructuring `Nullable<T>` (iOS)

1.4.65
 * #321 - Revert ES sink message property name to original value
 * #324 - Calculate ES index name from UTC timestamp
 * #315 - Remove Logentries SSL cert pinning (the cert changed)
 * #327 - Hide obsolete ES configuration methods
 * #311 - Accept multiple recipient addresses in the email sink

1.4.39
 * #289 - Elasticsearch sink improvements and new virtual methods on `JsonFormatter`

1.4.33
 * #302 - If a the last batch of log events sent by `PeriodicBatchingSink` was not full, wait the `period`
 * #304 - Make sure IO exceptions are suppressed by the `WriteTo.File()` configuration method

1.4.28
 * #303 - `AssemblyInformationalVersion` needs to track the package, not assembly, version, in order to play nicely with MSI

1.4.27
 * #283 - New solution targeting ASP.NET v.NEXT (when final, we'll refactor to give this first-class support)
 * #301 - _Serilog.Extras.Web_ improvements

1.4.23
 * Fixed some more NuGet packaging issues (_Serilog.Sinks.Splunk_ this time)

1.4.22
 * #297 - Update _loggly-csharp_ package dependency

1.4.21
 * Fixed some NuGet packaging issues (including a return to dependency groups for _Serilog.Sinks.Seq_)

1.4.18
1.4.17
1.4.16
 * New CI server used
 * #227 - Reduced default maximum destructuring depth and added configuration option
 * #245 - XML content escaping fixed in MSSQL sink
 * #272 - Allow underscores in property names

1.4.15
 * #259 - Update _loggly-sharp_ dependency (breaking change for _Serilog.Sinks.Loggly_, see PR for instructions)
 * #257 - Added _Serilog.Sinks.XSockets_
 * #246 - Changed target from _Profile78_ to (compatible but broader) _Profile259_
 * #250 - Allow an existing `MongoDatabase` instance to be used when configuring Mongo sink

1.4.14
 * #253 - Added `MessageTemplateFormatMethodAttribute`

1.4.13
 * #244 - Improvements to ElasticSearch sink, switch to just ElasticSearch.NET
 * #254 - Fix ElasticSearch dependency version
 * #249 - Track message template token indexes in parser to support tooling (binary-breaking)

1.4.12
 * #240 - Update TopShelf dependency
 * #243 - Caching in `AttributedDestructuringPolicy` closes over first seen object of a type rather than using the passed parameter
 * #242 - Update NLogSink to map `Verbose` level to `Trace` level in NLog
 * #229 - Created net40 version of Extras Topshelf
 * #236 - Ensure dictionary keys are quoted in JSON even when they're numeric
 * #237 - When `JsonFormatter` formats a dictionary of `<int, object>`, the key should be double quoted
 * #235 - Fixed serialization of dicationary keys in ES and similar sinks

1.4.11
 * #238 - Dynamic level switching

1.4.10
 * #225 - Ensure Azure Tablestorage rowkey is unique
 * #224 - Use UTC to generate partitionkey
 * #219 - .NET 4.0 support for Elastic Search
 * #221 - Exponential back-off for PeriodicBatchingSink

1.4.9
 * #213 - Check for null User.Identity when enriching events with usernames in ASP.NET
 * #216 - Updated to use Splunk TCP Writer

1.4.8
 * #204 - Basic HTTP authentication support for the CouchDB sink
 * #207 - Fixed typo in `DepthLimiter` error message
 * #209 - Update _Serilog.Sinks.Splunk_ to Splunk SDK 2.0 GA
 * #210 - Fixed string formatting in `PropertyBinder` error message

1.4.7
 * #192 - Additional enrichers for _Serilog.Extras.Web_
 * #202 - Batching mode for _Serilog.Sinks.AzureTableStorage_

1.4.6
 * Reintroduced fix from https://github.com/continuousit/seq-client/pull/19 dropped in project move

1.4.5
 * #179 - _Serilog.Sinks.Splunk_ updated for the Splunk SDK 2.0

1.4.4
  * Includes the _Serilog.Sinks.Seq_ sink, to write to the http://getseq.net event server

1.4.3
  * #169 - Added the _Serilog.Extras.DestructureByIgnoring_ package

1.4.2
  * #197 - Allow `EventSource` creation to be skipped when the source does not exist

1.4.1
  * #196 - Introduce `LogContext.Suspend()` to clear `LogicalCallContext` for cross-domain calls
