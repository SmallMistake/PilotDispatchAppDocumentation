# Data Passer

<blockquote>
<Strong>Summary</Strong>: Invisible Component that takes it's value from the initial data and passes that data when the form is submitted
</blockquote>

<!--<img src="./images/component_examples/string_example.png" alt="Icon Example">-->

## Schema Code

### Required Paramters
<strong>labelText</strong>: does not do anything (required to not crash database) <br>
<strong>attribute</strong>: new of value to pass

<blockquote>
<pre>
new DataPasserFormScreenItemWidget(
    new FormBuilderValidatorsText(true, 1, 50, true)
)
{
    labelText = "Log ID",
    attribute = "log_id"
},
</pre>
</blockquote>