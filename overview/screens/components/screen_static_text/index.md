# Screen String

<blockquote>
<Strong>Summary</Strong>: Displays the text exactly as entered on the Schema instead of changing based on data passed in
</blockquote>

<img src="./images/component_examples/string_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>textToShow</strong>: String to show

<blockquote>
<pre>
new ScreenStaticText(
    "Vessel"
)
</pre>
</blockquote>

### Additional Paramters
<strong>setFontSize</strong>: double<br>
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

<strong>setColorSet</strong>: ColorSet or ColorSetDefinition<br>
<pre>
    - Foreground color is used for text color
</pre>
