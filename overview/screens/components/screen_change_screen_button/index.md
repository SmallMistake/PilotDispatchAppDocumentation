# Screen Change Screen Button

<blockquote>
<Strong>Summary</Strong>: Creates a simple button for changing the screen
</blockquote>

<img src="./images/component_examples/change_screen_button_example.png" alt="Icon Example">

## Schema Code

### Required Paramters
<strong>field</strong>: type extra name<br>

<blockquote>
<pre>
new ScreenChangeScreenButton(
    "MobileTicketEditLink"
)
</pre>
</blockquote>

### Additional Paramters
<strong>setColorSet</strong>: ColorSetDefinition<br>
<pre>
    - Background color is used for button color
</pre>

<strong>setRouteType</strong>: RouteType<br>
<pre>
    -newPage
    -popup
</pre>

<strong>setWrapWithHero</strong>: bool<br>
<pre>
    - If true, the button will be wrapped with a hero
</pre>