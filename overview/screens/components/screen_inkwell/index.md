# Screen Inkwell

<blockquote>
<Strong>Summary</Strong>: Wraps a component with a clickable area
</blockquote>

<img src="./images/component_examples/hero_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>onTapFunction</strong>: InterchangableFunctions.Functions<br>
<strong>child</strong>: ScreenRowItem<br>
<strong>functionParameterJson</strong>: string<br>
<pre>
    - Additional paramters passed into api call
        -Example: "{\"phoneNumber\": \"COE{Phone1}\"}"
</pre>

<blockquote>
<pre>
new ScreenInkWell(
    onTapFunction: InterchangableFunctions.Functions.displayChildPopup,
    functionParameterJson: "",
    child: new ScreenContainer(
        ...
    )
    .setAllPadding(4)
)
</pre>
</blockquote>

### Additional Paramters
<strong>setAdditionalChild</strong>: ScreenRowItem<br>
<pre>
    - can be used by certain onTapFunctions like displayChildPopup to show this additional child
</pre>

<strong>setAttribute</strong>: string attributeName, string heroTag<br>
<pre>
    - attributeName: attribute name to use for hero tag
    - heroTag: used for when the click function is to open a hero
</pre>