# Notes   
> [!NOTE]   
> This file may not have any importance to the project, it's just a place to jot down my quick thoughts.   

* Write custom parser, with a stack of unclosed HTML tags. When a wrong closing tag is encountered, search its opening 
tag in the stack and close all contained tags implicitly. When the tag hasn't been opened, simply ignore the closing 
tag.   
* Make this usable for a browser, so integrate `js2py` or something similar and write/find a Python CSS parser. Always 
keep an eye on [js2py/README.md](https://github.com/PiotrDabkowski/Js2Py/blob/master/README.md) to see how to use it! 
Create a new `js2py.EvalJs` for each browsing context and pass in a `context` dict to replace `console` and create 
`document` and `location`, etc.!   
* 
