
{% assign id = {{page.id}} %}
source file: source/pages/\_includes/{{id}}-intro.md

{{site.data.structuredefinitions.[id].description}}

#### Mandatory Data Elements and Terminology

The following data-elements are mandatory (i.e data MUST be present).

**Each {{site.data.structuredefinitions.[id].type}} must have:**

1. A status
1. A measure report type hardcoded to "individual"
1. The reference to the [Measure]({{site.data.fhir.path}}measure.html)
1. The date the report was generated
1. The organization that reported the data
1. The reporting period
1. The results of the calculation (the Measure Scores)

Each {{site.data.structuredefinitions.[id].type}} *should* have ([Must Support](guidance.html#must-support)):

1. Separate subgroup calculations (stratifiers)
1. Reference to a reporting vendor using the DEQM [Reporting Vendor (STU3)] Extension
1. A certification identifier using the DEQM [Certification Identifier (STU3)] Extension

**Additional Profile specific implementation guidance:**

None

### Examples

{% include summary-measurereports.md %}

{% include link-list.md %}
