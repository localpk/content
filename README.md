# Local PK Content

This repository contains uncompiled content for Local.com.pk site. There are two important parts to it:

- All content are in [Markdown](https://guides.github.com/features/mastering-markdown/)
- The names and structure of the directories and files dictates the URL structure in the main website

In addition to Markdown, content can be written mixed with `HTML` and some Custom Components.

## Custom Components

[Custom components](https://using-remark.gatsbyjs.org/custom-components/) are basically ReactJS components. These are used here to produce custom UI elements from user generated contents that otherwise are not so straightforward to produce and sometime impossible. There are few things that need to be made sure when using these components:

- The value for all attributes are type string
- closing tag must be provided e.g. `<my-component />` is not allowed

Here is the list of Custom Components available for Local PK content:

---

### `<highlighted-numbers>`

*Attributes*

Name|Value
----|-----
data|stringified JSON

This component is used to display numbers prominently. A description is required against each number in the data.

*Example*

```html
<highlighted-numbers data='[{
  "numbers":"342", "description": "Total number of members", 
  "numbers":"272", "description": "Directly elected members"
}]'></highlighted-numbers>
```

Above code example renders following:

![image](https://user-images.githubusercontent.com/2131246/51764207-7e8b8200-20cc-11e9-8199-df07caf2b023.png)

---

Everyone is welcome to contribute, review and edit content.

- To add new content, add a new file and submit for review.
- To edit existing content, edit the file and submit for review.


## License
MIT License

## Copyrights
&copy; Local.com.pk - All rights reserved.

[![Analytics](https://ga-beacon.appspot.com/UA-50688851-1/localpk/content)](https://github.com/igrigorik/ga-beacon)
