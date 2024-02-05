# Add or Update new tool to the toolbox
The COGNIMAN Toolbox is structured according to the COGNIMAN Reference Architecture, which consists of seven layers. To add your tool to the portal, first, identify the layer to which your tool belongs and add the description file (in Markdown format) to the corresponding directory in the repository. The directories are underscore-prefixed:
- [_physicaltwin](/_physicaltwin): Physical Twin
- [_datalayer](/_datalayer): Data Layer
- [_digitaltwin](/_digitaltwin): Digital Twin 
- [_servicelayer](/_digitaltwin): Service Layer
- [_userinterface](/_userinterface): User Interface
- [_connectivity](/_connectivity): Connectivity and Intergration
- [_ssh](/_connectivity): SSH and Ethics

## Documentation Template
The tool description template can be found [here](/documentation/example_tool_template.md). An example of the description has been completed for SINDIT, which can be found [here](/_digitaltwin/sindit.md).

The **first section** of the template contains the meta-data (front matter) of the tool, which will be used to present the tool on the main page of the portal. The front matter is set between the triple-dashed lines:

```
---
title: "Your tool Title"
date: 2024-01-16T12:00:00+00:00
weight: 1
description: "Your tool short description goes here."
license: "https://img.shields.io/badge/License-Unlicense-lightgrey"
trl: "https://img.shields.io/badge/TRL-8-green"
link: "http://mytool.ex"
github: "https://github.com/tool"
---
```
- **Title**: Replace with the actual title of your tool.
- **Date**: Update the date to the current date or leave it as is.
- **Weight**: Define the order in which the tool will be shown in the category. To place the tool at the end of the list, please enter the current tool number plus 1.
- **Description**: Replace with a concise description of your tool.
- **License**: Replace the license URL with the appropriate license for your tool. Please refer to [License](#license) for more information.
- **TRL**: Update the TRL (Technology Readiness Level) badge link with the correct status. Please refer to [TRL](#trl) for more information.
- **Link** (optional): Replace with the official link to your tool's website. Otherwise, remove this entry.
- **GitHub** (optional): Replace with the official GitHub repository link for your tool. Otherwise, remove this entry.

The **second section** of the template is the content of the tool page. We use `markdown` to present the document, please refer to [this instruction](https://www.markdownguide.org/basic-syntax/) if you are not familiar with `markdown` syntax. You can have as many parts as possible in your tool page, but the following sections should be present:
- **Name**: Replace with the actual acronym or name of your tool.
- **Defined in Task**: Replace with the relevant task details.
- **Description**: Replace with a comprehensive overview of your tool. Describe interfaces, APIs, and the main purpose or functionality.
- **License**: Provide usage restriction and information about the license under which your tool is distributed.
- **Pilot**: Specify in which pilot(s) your tool is intended to be used.
- **References**: Include any relevant references or citations.

Once the tool description file has been pushed to the GitHub repository, the webpage will be compiled and deployed again. Please refer to the [Actions](https://github.com/COGNIMANEU/toolbox/actions) tab to check for any errors.

### Images
Store images inside the [images](/images) directory. Create a subdirectory named after your tool and place your images there. To use the images, use:
`![image_alt_text](/toolbox/images/link/to/your/image)` 

**Note:** Using the link syntax above, the image may not display on the GitHub interface, but it will be shown properly on the portal website.

### License
Select relevant license badge for your tool. Refer to [this page](https://gist.github.com/kofiav/c1059e1075b67582e86b07aa9759e20d) if you can not find your desired one.

#### Apache 2.0 License
[![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)  
`https://img.shields.io/badge/License-Apache%202.0-blue`

#### BSD 3-Clause License
[![License](https://img.shields.io/badge/License-BSD%203--Clause-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)  
`https://img.shields.io/badge/License-BSD%203--Clause-blue`

#### Creative Commons
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
`https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey`

#### Eclipse Public License 1.0
[![License](https://img.shields.io/badge/License-EPL%201.0-red.svg)](https://opensource.org/licenses/EPL-1.0)  
`https://img.shields.io/badge/License-EPL%201.0-red`

#### GNU GPL v3
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  
`https://img.shields.io/badge/License-GPL%20v3-blue`

#### IBM Public License Version 1.0
[![License: IPL 1.0](https://img.shields.io/badge/License-IPL%201.0-blue.svg)](https://opensource.org/licenses/IPL-1.0)  
`https://img.shields.io/badge/License-IPL%201.0-blue`

#### The MIT License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
`https://img.shields.io/badge/License-MIT-yellow`

#### Mozilla Public License 2.0
[![License: MPL 2.0](https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)  
`https://img.shields.io/badge/License-MPL%202.0-brightgreen`

#### The Unlicense
[![License: Unlicense](https://img.shields.io/badge/License-Unlicense-lightgrey)](http://unlicense.org)
`https://img.shields.io/badge/License-Unlicense-lightgrey`

#### Commercial Product
![License: Unlicense](https://img.shields.io/badge/License-Copyright%20%C2%A9-red)
`https://img.shields.io/badge/License-Copyright%20%C2%A9-red`

### TRL
Use the following badges:

![TRL](https://img.shields.io/badge/TRL-1-red)
`https://img.shields.io/badge/TRL-1-red`

![TRL](https://img.shields.io/badge/TRL-2-red)
`https://img.shields.io/badge/TRL-3-red`

![TRL](https://img.shields.io/badge/TRL-3-red)
`https://img.shields.io/badge/TRL-3-red`

![TRL](https://img.shields.io/badge/TRL-4-yellow)
`https://img.shields.io/badge/TRL-4-yellow`

![TRL](https://img.shields.io/badge/TRL-5-yellow)
`https://img.shields.io/badge/TRL-5-yellow`

![TRL](https://img.shields.io/badge/TRL-6-yellow)
`https://img.shields.io/badge/TRL-6-yellow`

![TRL](https://img.shields.io/badge/TRL-7-green)
`https://img.shields.io/badge/TRL-7-green`

![TRL](https://img.shields.io/badge/TRL-8-green)
`https://img.shields.io/badge/TRL-8-green`

![TRL](https://img.shields.io/badge/TRL-9-green)
`https://img.shields.io/badge/TRL-9-green`
