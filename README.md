# endnote-craft-workflow
Reference in markdown

Hey everyone! Welcome to my very first workflow. Hope you like it and would love to hear your feedback.

This workflow allows writing in-text citations in a markdown-esque fashion which can be converted into proper citations using EndNote’s Cite While You Write in Microsoft Word. There’s a bit of setup (and reading) required but I believe it’s worth it.

Users of Obsidian and other back-linking software with URL schemes could modify this to benefit them too (“See How It Works” for more information.)

# Required (Must be configured for use) (Red items in workflow)

- CRAFT SPACE ID: Found in the Craft deeplink. Please copy this into the workflow.
- File->Copy Formatted Keyboard Shortcut: Default should be Cmd+K. If not, change accordingly in the workflow.
- User-assigned hotkey
- Software: EndNote, Craft, Microsoft Word

Additional:


- Find Reference Updates: This should be done before running the workflow. The workflow splits  formatted citations objects by new lines and may fail if references are not updated.
- Temporary citation delimiters (EndNote Preferences->Temporary Citations): Default is { } but some may choose something different like [ ]. Please match these accordingly in the workflow if changed.

# Optional (but helpful)

- Craft Folder ID (optional - leave blank if not required): Found in the URL of the Craft Web Editor. Helpful for creating citation documents directly into your folder of choice.
- Attached EndNote referencing style (adapted version of Chicago 17th Footnote): If you would like to have all the important details including authors, title, doi link, and abstract, I’ve uploaded a EndNote referencing style which I use.
- Temporary citation page numbers (EndNote Preferences->Use field instead of record number->Pages): The record number will be used as default. This will work in the workflow but may cause issues if your EndNote library changes in the future. I recommend pages for longevity.
- Delay timers: These can be adjusted in the workflow. I suggest increasing the delay if there are errors or keeping them the same since shorter times can lead to not all references being created. 

# How it works


Select your references (multiple allowed) in EndNote and press the non-global hotkey (user-assigned in workflow) to copy the citations to the clipboard (these are passed as variables immediately so the clipboard manager option is not required.) Documents are created for each reference with the temporary/unformatted citation as the title and formatted citation as the body by using the Craft URL scheme “[craftdocs://createdocument?spaceId=&title=&content=&folderId=](craftdocs://createdocument?spaceId=&title=&content=&folderId=)“. When writing, use the @ symbol to search for the desired references which will be autofilled for you. Export to Microsoft Word, select all text, and remove hyperlinks (Cmd + Shift + F9) then turn on Instant Formatting in EndNote Cite While You Write. Voila! You have your references.

I recently tested this for a writing task and found it really helpful in keeping track of all my references since there is less friction, it is easier to remove or edit in-text citations, and the citations act as links to your notes and information.
