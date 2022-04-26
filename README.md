# Custom theme with ACF Page Builder
1. Before building a block consider if its a global content block, non-global block, or global block with the ability to be overridden on a page level.
1. Reduce the amount of blocks you create by incorporating block options into the block. For instance. A "text with media" block can have a "reverse order" option, to swap the image over to the left or right of the text, rather then creating an entirely new block. Furthormore, the media could be an image or a video, so we can build in an option for the block to support both image or video.
2. Always add default field values to the block fields when creating the blocks in the acf settings. 
3. Dont expose any class names or code in the block builder.
4. Always use the wysiwyg text editor instead of textarea field. 
5. Create an acf-json folder on your theme directory and keep changes to the acf field json under version control https://www.advancedcustomfields.com/resources/local-json/
https://www.awesomeacf.com/how-to-avoid-conflicts-when-using-the-acf-local-json-feature/
5. Hide the custom fields option on the production site https://www.awesomeacf.com/snippets/hide-the-acf-admin-menu-item-on-selected-sites/
6. Use Global block for Footer CTA Strip. If the content for this block changes at any point then updating this block on a website with 400 pages would be a mission.
7. Always check a field value exists before trying to display the value. php error will occur if the value does not exist. https://www.advancedcustomfields.com/resources/get_field/
8. Dont build breadcrumbs as a block, build it into the template.
9. Dont build inner page title / banners as a block, build it into the template.

How to build ACF block page builder system:
https://youtu.be/vq5ZTOQw7hg


[Back to main Dev Guidelines](https://github.com/pixelstorm/coding_guidelines_custom_builds)
