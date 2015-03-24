

# How to install this plugin? #
See http://help.eclipse.org/galileo/topic/org.eclipse.platform.doc.user/tasks/tasks-124.htm

Update Site: http://eclipse-fileencodinginfo.googlecode.com/svn/trunk/update/

# When will encoding be shown for a file? #
Encoding will be shown if the active editor supports the interface IEncodingSupport.
Editors supporting IEncodingSupport include Text Editor, HTML Editor, PHP Editor, Java Editor, XML Editor and etc.

# When will encoding be detected for a file? #
Encoding will be detected if the active editor implements the interface ITextEditor and the editor input is either IFileEditorInput or FileStoreEditorInput.
Editors implementing ITextEditor include Text Editor, HTML Editor, PHP Editor, Java Editor and etc.
Normally, the editor input should be either IFileEditorInput or FileStoreEditorInput.

# Under what conditions will alert be shown? #
Alert will be shown if
  1. The current encoding of the file is different from the detected encoding with the highest confidence, and the confidence of the detected encoding is larger than or equal to 50%, or
  1. The current encoding of the file is different from the detected encoding with the highest confidence, and the confidence of the current encoding is equal to 0%.

# What encodings can be detected? #
See http://userguide.icu-project.org/conversion/detection#TOC-Detected-Encodings

# Why disable the popup menu for changing encoding when the file is not saved? #
Because it seems that the encoding of an editor cannot be changed if it is dirty.
Although it is possible to change the encoding of the underlying workspace file, the new encoding will not be used to save the file.