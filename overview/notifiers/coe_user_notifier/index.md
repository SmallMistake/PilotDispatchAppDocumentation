# Coe User Notifier

<blockquote>
<strong>Summary:</strong> Notify listeners of changes to active user and schema
</blockquote>

## Overview
This notifier will mainly be called to check who is currently logged in. It also has functions releated to setting and reloading the schema.

## Common Functions

### List\<CoeUser> getUsers()
<pre>
  - Get all users that have quick logins saved
</pre>

### CoeUser? getActiveUser()
<pre>
  - Get user currently logged in
</pre>