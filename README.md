# NYU Blockchain Lab Website

Forked from [Hugo Academic CV Theme](https://github.com/HugoBlox/theme-academic-cv)

## Maintenance Notes

### Changing Affiliates Section

The affiliates section can easily be changed by altering one data file and replacing images with a uniform naming convention.

**Procedure**:

1. In [data/affiliates.yml](/data/affiliates.yml), the information for each user is set.
2. Simply copy paste new sections, or alter the current ones.
   - Note that there is a name, image, and socials field.
   - The image name here directly corresponds to the name of the image that is placed into the [images](/static/images/affiliates/) folder.
3. Images are stored in the **static** folder. For the affiliates section, they are in [static/images/affiliates](/static/images/affiliates/).
   - You do not necessarily have to keep the FirstLast.jpg naming convention, just make sure that in the [affiliates.yml](/data/affiliates.yml) file, the "image" field for each user corresponds to the name of the file placed here.

**Extra Note**:

This section was created using shortcode. The shortcode can be found at [layouts/shortcodes/teamSection.html](/layouts/shortcodes/teamSection.html). If you would like to add more fields for each user or alter the look, this is the place to go.

### Updating Events and Talks

The Upcoming and Past Talks section is based on the folder called [event](/content/event/).

**Procedure**:

1. Go to the [content/event](/content/event/) folder.
2. Each event has an index.md file that you can edit, which will reflect on both its own page (which you can access by clicking it) and on the card on the home screen.
   - Do **NOT** edit the "publish" date, unless you wish to have it automatically show up after a certain date.
3. To edit the date, edit the "date" field.
4. To edit the title and summary, simply replace the title and summary texts.
5. To add an event, just copy paste any of the current folders, such as 01-19, then edit the information inside.
   - You can name the folder whatever you like.
   - The section will automatically sort the events by date, newest first.
6. You can replace the image by replacing the featured.jpg file in each of the folders.

### Publications Section

The publications section is similar to the talks section, in that it generates content based on the folders inside [content/publication](/content/event/).

**Procedure**:

1. To add a publication, just copy paste one of the existing folders and edit the content.
   - You can name the folder whatever you like.
2. Optional: To add a citation, you can add a .bib file to the newly created folder.
   - Hugo will automatically generate a link for the citation on the card.
3. Optional: To add a PDF, you can also add a .pdf file to the newly created folder.
   - Hugo will automatically generate a link to the PDF on the card.
4. Optional: To add a thumbnail image, add an image called "featured.jpg" to the folder.

### Working Papers Section

The publications section is similar to the the publications section, in that it generates content based on the folders inside [content/post](/content/post/).

**Procedure**:

1. To add a working paper, just copy paste any of the folders inside the [content/post](/content/post/) folder and change the name to whatever you like.
2. Make sure to update the summary, link, dates, and authors inside.
3. To update or add a thumbnail, just add a 'featured.jpg/png' file inside it.
   - Yes, the file does need to be named 'featured'

### Global Styles

Global styles (so far only the font), are set in the header html as CSS styling. You can find it at [layouts/partials/hooks/head-end/custom.html](/layouts/partials/hooks/head-end/custom.html).

### Support and Hugo Blox Docs

- 👉 [**Get Started**](https://hugoblox.com/templates/)
- 📚 [View the **documentation**](https://docs.hugoblox.com/)
- 💬 [Chat with the **Hugo Blox Builder community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
