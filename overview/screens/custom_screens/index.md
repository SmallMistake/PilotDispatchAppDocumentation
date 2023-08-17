# Custom Screens

<blockquote>
<strong>Summary</strong>: A special screen type that allows you to specify premade widgets defined in the app
</blockquote>

## Overview
Many times you will need to create a page that would be too complicated to create with the schema. Custom screens come in to solve that problem. Once a custom screen has been created in the app it can be added to the schema almost like any other screen can be, except you will not be able to set the Row components.

<strong>Steps:</strong>
1) Create your widget in the app project
2) Add references to it in the custom widget functions
<pre>
    - user_home_screen.dart
    - screen_changer.dart
</pre>
3) Add a screen to the schema


## Example
#### screen_changer.dart
Add a reference in the switch statement here.
<blockquote>
<pre>
static Future<Widget> buildScreenWidget(...){
    ...
    switch (customWidget.customWidgetName) {
        case 'YouGlance':
            customScreenToGo = const ChartsDemoPage();
            break;
        case 'DemoWelcomeScreen':
            customScreenToGo =  const DemoWelcomePage(); 
        ...
    }
}
</pre>
</blockquote>

#### user_home_screen.dart
Add a reference in the switch statement here.
<blockquote>
<pre>
List<Widget> getScreensFromSchema(...){
    case 'customWidget':
        CustomWidgetStruct customWidget = screens[i] as CustomWidgetStruct;
        switch (customWidget.customWidgetName) {
        case 'YouGlance':
            result.add(const ChartsDemoPage());
            break;
        case 'DemoWelcomeScreen':
            result.add(const DemoWelcomePage());
            break;
        }
}
</pre>
</blockquote>

#### SchemaHelper.cs (DataService)
Add the screen definition here as you would any other page.
<blockquote>
<pre>
#region New Transportation Page
schemaResult.screens.Add(
    new ScreenCustomWidget(
        "Transportations",
        "NobraTransportationScreen",
        new List<string> { "All" },
        true
    )
    .setPageIcon(MaterialIconsEnum.local_taxi)
);
#endregion
</pre>
</blockquote>
