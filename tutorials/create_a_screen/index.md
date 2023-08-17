# How to Create a New Page

When releasing, we use a <strong>manual release</strong> system to ensure that both versions of the app go the the store at the same time and associations can be notified ahead of time. By following the steps listed below, you should be able to successfully release a new version of the app.

## Steps
1) Go to the SchemaHelper.cs file in your target association's DataService
2) Find the place where you would like your page to show up order wise
3) Use the template below add a new page to the schema

### Minimal Example

<blockquote>
<pre>
#region Assigned
schemaResult.screens.Add(
    new ScreenRegular(
        "Assigned",  //page Title
        "",          // url to call for topmost level
        0,           // Cardcolor (Outdated leftover)
        new List<ScreenRow>     // Primary Rows (This is where your main rows should go)
        {
            new ScreenRow(
                ...
            )
        },
        null,        // Detail Rows (On older schemas, if you want to add details to a card you would put your detail rows here)
        new List<string> { "All" },  // Allowed Users
    )
);
#endregion
</pre>
</blockquote>

4) Add the components you want in the primary rows region

### Additional Settings
5) Add additional settings after a page is setup based on what you need
<pre>
    - <strong>setType</strong>: PageTypes
        - <strong>regular</strong>: Uses multiple predefined rows that repeat a set of data
        - <strong>freeform</strong>: Only uses the first row so you have more control over layout
    - <strong>setPageIcon</strong>: MaterialIconsEnum
    - <strong>setVisibility</strong>: If visibility false, don't show on front pages rotation
    - <strong>setSelectable</strong>: allows card to be selectable
    - <strong>setUpdatable</strong>: adds an update timer to regular pages
</pre>