# Screen Column

<blockquote>
<Strong>Summary</Strong>: Wraps components with a Column
</blockquote>

<img src="./images/component_examples/column_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>children</strong>: List\<ScreenRowItem><br>
<blockquote>
<pre>
new ScreenColumn(
    children: new List<ScreenRowItem>
    {
        ...
    }
)
</pre>
</blockquote>

### Additional Paramters
<strong>setMainAxisAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>
<strong>setMainAxisSize</strong>: MainAxisSize<br>
<pre>
    - max
    - min
</pre>
<strong>setSpacing</strong>: int<br>