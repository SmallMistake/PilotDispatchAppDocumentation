# Screen Label

<blockquote>
<Strong>Summary</Strong>: Wraps a child with a label object
</blockquote>

<img src="./images/component_examples/label_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>labelText</strong>: shortcut for setting the labelWidget to a string<br>
<strong>labelWidget</strong>: advanced method of seeting the label to an object<br>
<strong>childWidget</strong>: child to be wrapped by label

<blockquote>
<pre>
<strong>String Shortcut</strong>
new ScreenLabel(
    "L.f.",
    new ScreenString(
        "LastFinishDateTime"
    )
),

<strong>or</strong>

<strong>Advanced Method</strong>
new ScreenLabel(
    labelWidget: new ScreenIcon(
        MaterialIconsEnum.phone
    ).setColorSet(
        ColorSetDefinition.staticBlue
    ),
    childWidget: new ScreenString(
        "",
        "Phone1"
    ).setRegexFormat(
        RegexFormat.nationalTelephoneNumber
    )
)
</pre>
</blockquote>

### Additional Paramters
<strong>setAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>

<strong>setEmptyListener</strong>: List\<String><br>
<pre>
    - Shortcut for wrapping a label with an empty listener. If all passed strings are empty, component will be hidden
</pre>
