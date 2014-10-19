Scholdoc-Template
===================

### Scholdoc default conversion templates for HTML5, LaTeX, and Docx output

**Current schema version:** [0.1][scholmd-schema]

Scholdoc templates, forked from [`pandoc-templates`](https://github.com/jgm/pandoc-templates).

All Scholdoc-specific templates start with `scholmdTemplate`. Extensions denote the intended output target. Template names ending in `_bodyOnly` gets if you similarly append `_bodyOnly` when specifying Scholdoc output format. For example, specifying `--to=html_bodyOnly`  will use the `scholmdTemplate_bodyOnly.html5` (note that Scholdoc outputs to HTML5 only).

The template syntax follow the [Pandoc template syntax][pandoc-template]. Variables are surrounded by single dollar-signs, like `$VARIABLE_NAME$`. The template also understand a very limited set of control-flow logic, including `$if(VARIABLE)$ ... $else$ ... $endif$`  to check for existence and `$for(VARIABLE)$ ... $endfor$` to iterate over a list.

For more information, consult the [template section][pandoc-template] section of the Pandoc guide.

If you use custom templates, we recommend forking this repository,
so that you can integrate changes to the default templates in future
Scholdoc releases.

[pandoc-template]: http://johnmacfarlane.net/pandoc/README.html#templates
[scholmd-schema]: http://scholarlymarkdown.com/Scholarly-Markdown-HTML-Schema.html

### Licensing

All of the templates in this repository are dual licensed, under both
the GPL (v2 or higher, same as pandoc) and the BSD 3-clause license
(included below).

----

Copyright (c) 2014, Tim T.Y. Lin  
Copyright (c) 2014, John MacFarlane

All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.

    * Redistributions in binary form must reproduce the above
      copyright notice, this list of conditions and the following
      disclaimer in the documentation and/or other materials provided
      with the distribution.

    * Neither the name of John MacFarlane nor the names of other
      contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
