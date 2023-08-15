
# App Structure Overview

The PilotDispatch App is based around a Schema design.

Each time the user logs in, the app calls to the associations servers to get the current schema that matches their phone's minimum schema version. This means that multiple schemas can be on the site at a time if some users have different versions of the app.

## The Schema

The schema is a json that is passed to the app. It is usually set via the Schema_Designer_Json component on the association's website. Said component uses the file SchemaHelper.cs in the DataService to create a new Schema.

<blockquote>
The Schema is made up of only two main pieces: <strong>Screens</strong> and <strong>Forms</strong>
</blockquote>

## Screens

Screens are the primary building block of the app. They represent any page where data entry is not the primary focus.

[**Learn more about Screens**](./overview/screens/index)
## Forms

Forms are like screens except that they specialize on data entry. They do not have as much visual flexiblitiy as screens, but they offer better data submission functionallity.

[**Learn more about Forms**](./overview/forms/index)