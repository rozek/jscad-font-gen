##  --- jscad-font-gen ---

A utility to convert single-line svg fonts to jscad font data. It can create modules for importing or it can inject the font data directly into a jscad file.

Installation ...
```
git clone git@github.com:mark-hahn/jscad-font-gen.git
cd jscad-font-gen
npm i
```

Command-line options
* -i regex  

  - Limit letters to ones that match the regex.
  - Defaults to [\\x20-\\x7E] which matches ascii characters that jscad can handle
  - Remember to enclose it in single-quotes if it has backslashes or spaces.

* -m
  - Flag that indicates the output should include code to make the file an importable module.
  - If not specified then font data is injected directly into the output file.

* -i input-path.svg
  - The svg file to convert or a directory containing svg files.

* -o output-path.js

Usage
```
  cd jscad-font-gen
  node index.js 
```
