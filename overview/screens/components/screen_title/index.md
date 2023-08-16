# Screen Title

<blockquote>
<Strong>Summary</Strong>: Wrap an object with dividers to make a title visual
</blockquote>

<img src="./images/component_examples/title_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>child</strong>: ScreenRowItem

<blockquote>
<pre>
new ScreenTitle(
    child: new ScreenString(
        "Vessel_Name"
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
