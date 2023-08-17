# Text Field Numeric

<blockquote>
<Strong>Summary</Strong>: Text Field that only allows for numbers to be entered.
</blockquote>

<img src="./images/form/numeric_example.png" alt="Numeric Example">

## Schema Code

### Required Paramters
<strong>labelText</strong>: label <br>
<strong>attribute</strong>: name of value to pull from

<blockquote>
<pre>
new FormBuilderTextFieldNumeric(
    new FormBuilderValidatorsNumeric(true, 0, 500)
)
{
    labelText = "Draft Feet",
    attribute = "draftft"
},
</pre>
</blockquote>