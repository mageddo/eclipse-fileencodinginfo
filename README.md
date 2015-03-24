# eclipse-fileencodinginfo
Automatically exported from code.google.com/p/eclipse-fileencodinginfo

This Eclipse plugin adds the following features to Eclipse:

    Show the encoding of the current editing text file in the trim area.

    Use the ICU component to detect the possible encodings of the current editing text file, and alert you to change encoding if the encoding may not be set correctly.

    Allow you to change encoding through the popup menu.

I work in an environment where I need to access remote files (which may be of UTF-8 or Big5) through the Remote System Explorer, but Eclipse do not detect the file encoding for me and will corrupt the file if I forget to set the file encoding properly, so I write this plugin.

If you use Remote System Explorer, you may want to try My RSE Extensions. 
