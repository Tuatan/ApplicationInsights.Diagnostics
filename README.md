[![Nuget](https://img.shields.io/badge/nuget-v1.0.50140-green.svg?style=plastic)](http://nuget.org/packages/tx.core)
# ApplicationInsights.Diagnostics

[![Join the chat at https://gitter.im/Tuatan/ApplicationInsights.Diagnostics](https://badges.gitter.im/Tuatan/ApplicationInsights.Diagnostics.svg)](https://gitter.im/Tuatan/ApplicationInsights.Diagnostics?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

ApplicationInsights.Diagnostics allows yu to get a list of all the Application Insights verbose traces. 

In LINQPad you would do the following:

- Run LINQpad as administartor
- Create new query in LINQpad
- Add ApplicationInsights.Diagnostics nuget package (or just open this linq file if you do not have premium features enabled)
- Add namespaces: System.Reactive.Linq, ApplicationInsights.Diagnostics.
- Write the following query: 
``` csharp
DiagnosticObservable.Create().Select(i => i.FormattedMessage)
```

You could find more information how to use it [here](http://tuatan.github.io/blog/2015/04/16/diagnostic-of-applicationinsights-sdk/).
