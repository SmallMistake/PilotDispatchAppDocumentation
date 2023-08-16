# Screen Wrap

<blockquote>
<Strong>Summary</Strong>: Wraps a component with a Wrap
</blockquote>

<img src="./images/component_examples/string_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>children</strong>: List\<ScreenRowItem><br>
<blockquote>
<pre>
new ScreenWrap(
    children: new List<ScreenRowItem>
    {
        ...
    }
)
</pre>
</blockquote>

### Additional Paramters
<strong>setHorizontalAlignment</strong>: AlignmentType<br>
<pre>
    - start
    - center
    - end
    - spaceAround
    - spaceEvenly
</pre>