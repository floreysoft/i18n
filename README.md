# The I18n Component
Developing a localized application is already supported by the Java language in a comfortable way. This package adds the feature of localized message bundles that group localized messages together. Think of a localized error description that consists of title, text, summary and error details. These localized messages can be grouped together to form a localized error bundle.
This might be very useful in order to display these entries of the error description to the user in different ways. In a web based environment it might make sense to format the error title in a different way than the details. When logging error messages it might be useful to use different log levels for the error summary or the error details.
Localized exceptions make use of this detailed error description. Have a look at the examples to see localized exception in action.
A MessageManager takes care of handling different pluggable MessageProviders that deal with different message sources. This allows you to define the messages in your favourite format and enables easy migration to the i18n-component.
Each MessageProvider can handle a number of different resources so that a bunch of messages defined in a single resource (e.g. a file) can be updated or uninstalled.

# Features at a glance
Messages that are part of an entity can be grouped together using bundles
The localization takes place lately when accessing message entries. This allows printing the same message in different languages.
Localized exceptions enable a java applications to provide detailed localized exception messages.
XML and ResourceBundle based message providers
Pluggable custom message providers enable access to existing data sources.
