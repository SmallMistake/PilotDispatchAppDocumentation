# Screen Padding

<blockquote>
<Strong>Summary</Strong>: Wraps a component with Padding
</blockquote>

<img src="./images/component_examples/padding_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>child</strong>: ScreenRowItem<ScreenRowItem><br>
<blockquote>
<pre>
new ScreenPadding(
    child: ...
)
</pre>
</blockquote>

### Additional Paramters
<strong>setPadding</strong>: PaddingDirection paddingDirection, int paddingAmount<br>
<pre>
    -These calls can be chained to set specific paddings
    - top
    - left
    - right
    - bottom
</pre>
<strong>setAllPadding</strong>: int<br>
<strong>setScreenPadding</strong><br>
<pre>
    - Coomon shortcut for setting padding for screens
</pre>