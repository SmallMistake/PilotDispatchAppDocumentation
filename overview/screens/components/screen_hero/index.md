# Screen Hero

<blockquote>
<Strong>Summary</Strong>: Wraps a component with a Hero that can be used when expanding for more details
</blockquote>

<img src="./images/component_examples/hero_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>heroTag</strong>: string<br>
<pre>
    - Tag used by Hero to ensure that duplicate Heroes do not conflict
    - If you have a hero on each row make sure to vary it with unique data
</pre>
<strong>child</strong>: ScreenRowItem<br>

<blockquote>
<pre>
new ScreenHero(
    "shipCardCOE{RowNumber}",
    child: new ScreenCard(
        ...
    )
)
</pre>
</blockquote>

### Additional Paramters
None