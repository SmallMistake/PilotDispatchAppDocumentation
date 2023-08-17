# Error Reporting

<blockquote>
Error Reporting can be handled in the app and in DataServices
</blockquote>

## Error Report Helper
This class can be used to send reports from the app to the associations server.

#### Future\<Map\<String, dynamic>> createErrorValues
Call this function to create a list of values to be sent to the server

#### Future\<bool> sendErrorReport
Call this function - usually pass in the values created by the function createErrorValues - to send a reprot to the association server

## Error Report Popup
Use this class as a popup to ask the user if they want to add details to the error report.

## Examples
#### Send Report with User Popup
<blockquote>
<pre>
await showDialog(
    barrierDismissible: false,
    context: context,
    builder: (context) {
        return ErrorReportPopup(response);
    },
);
</pre>
</blockquote>

#### Send Report from App Manually
<blockquote>
<pre>
ErrorReportHelper.createErrorValues(
    Provider.of<CoeUserNotifier>(context, listen: false).getActiveUser(),
    'Error On Form Post',
    e.toString(),
    stacktrace.toString(),
).then((errorReport) {
    ErrorReportHelper.sendErrorReport(
        context, 
        errorReport
    );
});
</pre>
</blockquote>