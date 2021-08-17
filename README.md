![Screen Shot 2021-08-18 at 07 57 31](https://user-images.githubusercontent.com/89093232/129806358-e424aa98-f75e-4c1a-884d-f0d5b14d8870.png)
![Screen Shot 2021-08-18 at 07 58 43](https://user-images.githubusercontent.com/89093232/129806378-7406a4e3-ebe8-4903-acce-f1fe3a865780.png)
Hey everyone! Welcome to my very first workflow. Hope you like it and would love to hear your feedback.

This workflow allows writing in-text citations in a markdown-esque fashion which can be converted into proper citations using EndNote’s Cite While You Write in Microsoft Word. There’s a bit of setup (and reading) required but I believe it’s worth it.

Users of Obsidian and other back-linking software with URL schemes could modify this to benefit them too (“See How It Works” for more information.)

![Document Page](https://user-images.githubusercontent.com/89093232/129806573-799b6357-ccb3-4e91-87f2-98808959c8c8.png)

![In-Text Citation](https://user-images.githubusercontent.com/89093232/129806584-8d732927-1f50-4574-81c8-a52dc08a2a38.png)


# Required (Must be configured for use) (Red items in workflow)

- CRAFT SPACE ID: Found in the Craft deeplink. Please copy this into the workflow.
- File->Copy Formatted Keyboard Shortcut: Default should be Cmd+K. If not, change accordingly in the workflow.
- References must be in the form of {ref1} or {ref1;ref2;ref3} , where { } are temporary citation delimiters***
- User-assigned hotkey
- Software: EndNote, Craft, Microsoft Word

Additional:


- Find Reference Updates: This should be done before running the workflow. The workflow splits  formatted citations objects by new lines and may fail if references are not updated.
- ***Temporary citation delimiters (EndNote Preferences->Temporary Citations): Default is { } but some may choose something different like [ ]. Please match these accordingly in the workflow if changed.

# Optional (but helpful)

- Craft Folder ID (optional - leave blank if not required): Found in the URL of the Craft Web Editor. Helpful for creating citation documents directly into your folder of choice.
- Attached EndNote referencing style (adapted version of Chicago 17th Footnote): If you would like to have all the important details including authors, title, doi link, and abstract, I’ve uploaded a EndNote referencing style which I use. I wrote APD (Academic Paper Reference - v fancy) into the reference to help searching for them in Craft but that can obviously be removed.
- Temporary citation page numbers (EndNote Preferences->Use field instead of record number->Pages): The record number will be used as default. This will work in the workflow but may cause issues if your EndNote library changes in the future. I recommend pages for longevity.
- Delay timers: These can be adjusted in the workflow. I suggest increasing the delay if there are errors or keeping them the same since shorter times can lead to not all references being created. 

# How it works


Select your references (multiple allowed) in EndNote and press the non-global hotkey (user-assigned in workflow) to copy the citations to the clipboard (these are passed as variables immediately so the clipboard manager option is not required.) Documents are created for each reference with the temporary/unformatted citation as the title and formatted citation as the body by using the Craft URL scheme “[craftdocs://createdocument?spaceId=&title=&content=&folderId=](craftdocs://createdocument?spaceId=&title=&content=&folderId=)“. When writing, use the @ symbol to search for the desired references which will be autofilled for you. References should be in the form {ref1} or {ref1;ref2;ref3} . Export to Microsoft Word, select all turn, and remove hyperlinks (Cmd + Shift + F9) then text on Instant Formatting in EndNote Cite While You Write. Voila! You have your references.

I recently tested this for a writing task and found it really helpful in keeping track of all my references since there is less friction, it is easier to remove or edit in-text citations, and the citations act as links to your notes and information.
