
# tag-input

  Turns a text input element into a pretty tags input.
  Enables you to work with any MVC framework using simple events or you can get the tags from the inner model.

  ``` javascript
    var TagInput = require('tag-input');

    var taginput = TagInput(document.getElementById('tags'))

    taginput.on('add', function (tag) {
      console.log(tag + ' added')
      console.log(taginput.tags())
    })

    taginput.on('remove', function (tag) {
      console.log(tag + ' removed')
      console.log(taginput.tags())
    })

  ```

## css
  The pseudo input decoration is basic for now.
  You can extend it by adding to taginputContainer class.

## api
  ### TagInput(input)
    binds to a text input element

  ### addtag(tag)
    adds a tag to the tag input from js

  ### removetag(tag)
    removes a tag from the tag input from js

  ### event: 'add'
    Called when a tag is added

  ### removed: 'removed'
    Called when a tag is removed`

