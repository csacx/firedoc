
# firedoc 1.0.1

Fire Doc, Fireball-x&#x27;s JavaScript Documentation engine forked from YUI.

### `Utils` Class


Defined in: [lib/utils.js:11](../files/lib/utils.js.js)

Module: [yuidoc](../modules/yuidoc.md)




Utilities Class

### Index



##### Methods

  - [`escapeHTML(html)`](#method-escapehtmlhtml)
  - [`fixType(t)`](#method-fixtypet)
  - [`getDirs(dir)`](#method-getdirsdir)
  - [`getLayouts(dir)`](#method-getlayoutsdir)
  - [`getPage(pagePath)`](#method-getpagepagepath)
  - [`getPages(dir)`](#method-getpagesdir)
  - [`getPartials(dir)`](#method-getpartialsdir)
  - [`getProjectData([dir=process.cwd()])`](#method-getprojectdatadirprocess.cwd)
  - [`localize(str)`](#method-localizestr)
  - [`markdownLink(str)`](#method-markdownlinkstr)
  - [`prepare(inDir, options, callback)`](#method-prepareindir-options-callback)
  - [`unindent(content)`](#method-unindentcontent)
  - [`validatePaths(paths, [ignore=false])`](#method-validatepathspaths-ignorefalse)
  - [`webpath(url)`](#method-webpathurl)





### Details




<!-- Method Block -->
#### Methods


##### method: `escapeHTML(html)`

Escapes HTML characters in _html_.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:31](../files/lib_utils.js.md#l31) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- html <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> String to escape.


##### method: `fixType(t)`

Takes a type string and converts it to a "First letter upper cased" type. e.g. `(string -> String, object -> Object)`

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:452](../files/lib_utils.js.md#l452) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- t <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> The type string to convert


##### method: `getDirs(dir)`

Walks the tree from this dir and returns all the subdirs

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:338](../files/lib_utils.js.md#l338) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Array" class="crosslink external" target="_blank">Array</a> 

###### Parameters
- dir <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> The dir to begin at


##### method: `getLayouts(dir)`

Like `getPages()`, but returns only the files under the `layout/` subdirectory
of the specified _dir_.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:63](../files/lib_utils.js.md#l63) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 

###### Parameters
- dir <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Directory path.


##### method: `getPage(pagePath)`

Loads and returns the content of the specified page file.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:76](../files/lib_utils.js.md#l76) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> | null 

###### Parameters
- pagePath <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Path to a single `.handlebars` page.


##### method: `getPages(dir)`

Loads pages (files with a `.handlebars` extension) in the specified directory and
returns an object containing a mapping of page names (the part of the filename)
preceding the `.handlebars` extension) to page content.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:91](../files/lib_utils.js.md#l91) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 

###### Parameters
- dir <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Directory path.


##### method: `getPartials(dir)`

Like `getPages()`, but returns only the files under the `partial/` subdirectory
of the specified _dir_.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:125](../files/lib_utils.js.md#l125) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> 

###### Parameters
- dir <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Directory path.


##### method: `getProjectData([dir=process.cwd()])`

Walk the directory tree to locate the yuidoc.json file.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:224](../files/lib_utils.js.md#l224) |

###### Parameters
- dir Path The directory to start from


##### method: `localize(str)`

Localize the string via current Y.options

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:492](../files/lib_utils.js.md#l492) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- str <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> the original string that you want to input


##### method: `markdownLink(str)`

convert string to markdown link

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:536](../files/lib_utils.js.md#l536) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- str <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> the original string that you want to input


##### method: `prepare(inDir, options, callback)`

Mix/merge/munge data into the template.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:139](../files/lib_utils.js.md#l139) |

###### Parameters
- inDir <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> The starting directory
- options <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> The `options` for the meta data.
- callback Callback The callback to excecute when complete
	- err <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Error" class="crosslink external" target="_blank">Error</a> 
	- options <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Merged options.


##### method: `unindent(content)`

Normalizes the initial indentation of the given _content_ so that the first line
is unindented, and all other lines are unindented to the same degree as the
first line. So if the first line has four spaces at the beginning, then all
lines will be unindented four spaces.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:44](../files/lib_utils.js.md#l44) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- content <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Text to unindent.


##### method: `validatePaths(paths, [ignore=false])`

Make sure all the paths passed are directories and that they are not in the ignore list.

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:364](../files/lib_utils.js.md#l364) |

###### Parameters
- paths <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Array" class="crosslink external" target="_blank">Array</a> The array of paths to validate
- ignore <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> A string to call `.indexOf` on a path to determine if it should be ignored


##### method: `webpath(url)`

Produces a normalized web path by joining all the parts and normalizing the
filesystem-like path into web compatible url.
Supports relative and absolute paths.
Courtesy of [Mojito's utils](https://github.com/yahoo/mojito/)

| meta | description |
|------|-------------|
| Defined | [lib/utils.js:474](../files/lib_utils.js.md#l474) |
| Return 		 | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> 

###### Parameters
- url <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Array" class="crosslink external" target="_blank">Array</a> | <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String*</a> the list of parts to be joined and normalized



