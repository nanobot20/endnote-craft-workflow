Hey everyone! Welcome to my very first workflow. I hope it helps the writing experience and am open to any suggestions for improvement.

Import your EndNote citations into Craft for markdown-esque referencing which can be easily and properly formatted with EndNote’s Cite While You Write in Microsoft Word. Users of Obsidian and other back-linking software with URL schemes could modify this to benefit them too (See “Usage” for more information.)

# Install


Download the Alfred Workflow file and input your Space ID (required) and Folder ID (optional). Found within the Craft deeplink and Web Editor URL.

Assign non-global hotkey to trigger the workflow.

In EndNote, confirm the following settings or change in Alfred or EndNote accordingly. 


- Cmd+K = Edit->Copy Formatted. 
- Temporary citation delimiter (in EndNote Preferences->Temporary Citations) matches the workflow settings (default { } )
- Recommended (optional): Set EndNote Preferences->Use field instead of record number->Pages. The default is record number which will work but may not age well if you change your EndNote library in the future.
- Citation format: This workflow will import your selected referencing style as content. I’ve uploaded a referencing style (modified version of Chicago 17th Footnote) which includes the author names, titles, doi link, abstract, and other details if available and helps me keeping track of all my notes.

Software:


- EndNote
- Craft
- Word (for export)

# Usage


## Import

1. Select references (as many as desired.) Recommended to Find Reference Updates prior to next step.
2. Trigger hotkey
3. Sit back as citations are imported. Temporary/unformatted citations and formatted citations are copied to clipboard (clipboard manager is not required as variables are passed immediately.)  Documents are created for each reference with the temporary/unformatted citation as the title and formatted citation as the body by using the Craft URL scheme “[craftdocs://createdocument?spaceId=&title=&content=&folderId=](craftdocs://createdocument?spaceId=&title=&content=&folderId=)“.

![Reference Import](https://user-images.githubusercontent.com/89093232/129854668-1bf1ad42-fe7a-40ef-a25a-7689402597da.png)


## Markdown Citations


Use the reference format {ref} or {ref1;ref2;ref3;…;refx} where { } are your temporary citation delimiters:


1. Type {@
2. Reference away

![In-Text Citations](https://user-images.githubusercontent.com/89093232/129854647-d73a158b-3132-42be-b261-5488a22916e9.png)


## EndNote Cite While You Write

1. Export to Word
2. Select all text (Cmd+A)
3. Remove hyperlinks (Cmd+Shift+F9)
4. Turn on instant formatting in the EndNote Cite While You Write ribbon

![Formatting in Word](https://user-images.githubusercontent.com/89093232/129854685-fd3bee81-a4fa-4a3e-adc2-3e15a976c39b.png)

Viola! A Crafty method for referencing!
