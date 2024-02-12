# Configuration

AppInsights Log Level can be configured in appsettings.json

```
"Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Information"
    },
    "ApplicationInsights": {
      "LogLevel": {
        "Default": "Warning",
        "Malue.App": "Trace",

        "Microsoft": "Warning",
        "Microsoft.Hosting.Lifetime": "Information"
      }
    }
  }
```

LogLevels can be set to Category prefix granularity.

Consider the following code snippet injecting a logger into the EvaluationTemplates page"
`@inject ILogger<Malue.App.UI.Blazor.Pages.EvaluationTemplates> Logger`

The Category of this logger is the type `Malue.App.UI.Blazor.Pages.EvaluationTemplates`.
By setting `"Malue.App": "Trace"` I am setting all loggers with a Category prefixed with `Malue.App` to Trace LogLevel.

This is useful if I want to limit certain Microsoft Trace or Warning logs but want to make exceptions for certain high priority components.

As such it is best practice to use the current class Type as the Category Type when injecting your logger.

You can then use the logger as follows in your code to log messages at varying Log Levels:
```
Logger.LogWarning("Templates Page - Warning");
Logger.LogInformation("Templates Page - Info");
```


### Valid LogLevels:
- Critical
- Error
- Warning
- Information
- Trace
- None

