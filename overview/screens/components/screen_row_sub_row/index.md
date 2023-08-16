# Screen Row Sub Row

<blockquote>
<Strong>Summary</Strong>: Creates a Row inside of a Screen Row
</blockquote>

<img src="./images/component_examples/hero_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>children</strong>: List\<ScreenRowItem><br>
<blockquote>
<pre>
new ScreenRowSubRow(
    new List<ScreenRowItem>
    {
        ...
    }
)
</pre>
</blockquote>

### Additional Paramters
<strong>setVerticalAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>
<strong>setHorizontalAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>
<strong>setSpacingBetweenChildren</strong>: int<br>