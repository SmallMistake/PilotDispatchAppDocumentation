# Screen String

<blockquote>
<Strong>Summary</Strong>: Displays a formattable string as text
</blockquote>

<img src="./images/component_examples/string_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>field</strong>: field from data that will be used to fill this componenet

<em> title: is not required but is a hold over from when it was. Remove eventually</em>

<blockquote>
<pre>
new ScreenString(
    "LastFinishDateTime"
)
</pre>
</blockquote>

### Additional Paramters
<strong>setFontSize</strong>: double or int<br>
<strong>setFontWeight</strong>: FontWeight<br>
<pre>
    - thin
    - regular
    - bold
</pre>
<strong>setAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>

<strong>setRegexFormat</strong>: RegexFormat<br>
<pre>
    - Use this to select a common simple Regex Expressions
        - nationalTelephoneNumber
</pre>

<strong>setCustomFormat</strong>: string<br>
<pre>
    - Use this with the Coe Regex Helper - TODO Link to COE Regex Helper Here - to define more advanced custom Regex Expressions
</pre>

<strong>setColorSet</strong>: ColorSet or ColorSetDefinition<br>
<pre>
    - Foreground color is used for text color
</pre>
