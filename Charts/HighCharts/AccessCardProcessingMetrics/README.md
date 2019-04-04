## Access Card Processing Metrics

This weblet renders various access card processing time metrics per day as a line chart that is powered by [High Charts](https://www.highcharts.com/docs/) library.

#### View Components

* **Weblet** - renders access card processing time metrics as line chart

  ![Access Card Processing Metrics](images/s1.PNG)

#### Backend Components

* **SandboxBackend** - _Lucy model_ that provides data for the view to render with the following action sequences,
  * **AccessCardProcessingTime** - returns processing time metrics