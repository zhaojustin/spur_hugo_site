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

### Global Styles

Global styles (so far only the font), are set in the header html as CSS styling. You can find it at [layouts/partials/hooks/head-end/custom.html](/layouts/partials/hooks/head-end/custom.html).

### Support and Hugo Blox Docs

- 👉 [**Get Started**](https://hugoblox.com/templates/)
- 📚 [View the **documentation**](https://docs.hugoblox.com/)
- 💬 [Chat with the **Hugo Blox Builder community**](https://discord.gg/z8wNYzb) or [**Hugo community**](https://discourse.gohugo.io)
