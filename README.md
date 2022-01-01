# How to update Schefens Archive

1. Go to the `schefens.html` file in a text editor, and copy the code for the previous year,
it will begin with an `<h1>` tag which contains the name of the hosts and a link
to the show. Below the `</h1>` closing tag will be a `<div>` tag, make sure to include
only in your copy everything up to the next closing `</div>` tag. You can tell it will
be the right one if it is on the same indentation level.
2. Paste this code above the `<h1>` tag. Now edit the newly pasted code within the `<h1>`
tag to include the new link to the current Schefens (within the `<a>` tag's `href` attribute),
as well as updating the name of the show and the hosts in the body of the `<a>` tag.
3. The `<table>` tag below contains the table containing all the row and columns.
The `<tr>` tag contains each column. Within it, the `<th>` tags contain the rows within
the columns. Start editing the `<th>` tags with the new winners and the videos they're in.
It is laid out like this:
```
<tr>
    <th>Award</th>
    <th>Winner</th>
    <th>Video</th>
</tr>
```
So if you want to edit the award name, edit the first `<th>` tag. If you want to edit
the winner name, edit the second, and if you want to edit the video name edit the third.
Whitespace does not matter, you can indent to make your code look cleaner and it'll still
display the same.

Each Schefens often has new awards, or removes an old one. If this happens, you can add
or remove an entire `<tr>` tag. If you add one, ensure that there are exactly three
`<th>` tags within each `<tr>`. Even if one is blank (such as Video), include an empty
`<th></th>` set.

If you need to add the `<` or `>` symbol for a video name, it will not work as it interferes
with HTML rules. To get around this, substitue the symbol for the entity code below:
`<`: `&lt;`
`>`: `&gt;`
Example: this video is called "I <3 Aliens". To print this properly:
```
<th>I &lt;3 Aliens</th>
```

4. Now that your code is finished, you need to insert it into the website. To do this,
go to Wix and go to the Schefens Archive page. Click on the HTML entity in the center of
the page (it will contain the tables), and a button will appear "Edit Code." Click that,
and there will be a text box with the label "Add your code here (HTTPS only)" Copy your code from
wherever you were editing it, then paste it into that box.
5. Scroll to the bottom of the page now, the page will need to be stretched now to fit the older
content which is now hidden. Put your cursor on the bottom of the HTML entity and above
the NUTV copyright information section. You will see a resizing icon. Pull your cursor down until
the HTML entity grows enough that you can see the oldest Schefens info in the archive (Fall 2017).
6. Click Publish on the top right of your window.
7. Update this GitHub repository by clicking the edit icon while viewing `schefens.html`. An editor
will appear. Replace the code in it with the code in your text editor.
