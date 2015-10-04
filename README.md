# multilanguage
This is the multilanguage.sty package for LaTeX

The solution is based upon [TEX StackExchange answer](http://tex.stackexchange.com/questions/5076/is-it-possible-to-keep-my-translation-together-with-original-text/31401#31401)

Usage:
`% MULTILINGUAL SUPPORT`
`\usepackage[italian,englishlithuanian]{babel}` %enables babel to every lang supported by your document
`\usepackage{multilanguage}` % import the file with the above definitions
`%\setdoclang{it}{italian}` % set short and long language codes
                         % the second one must be known by babel
`%\setdoclang{en}{english}`
`\setdoclang{lt}{lithuanian}`
`% END MULTILINGUAL SUPPORT`
...
% Sections, subsections, subsubsections:
`\sectionlang{it}{Sezione 1}` % in the first parameter you can freely use
                            % both short or long language codes
`\sectionlang{english}{Section 1}`

% Strings that are displayed only in a certain language
`\lang{it}{Questa stringa appare solo in italiano.}`
`\lang{en}{This string shows up only in English.}`
`\lang{lt}{Ši eilutė bus tik lietuviškame tekste.}`
% When you have only two languages, you can simply rely on this if-else
% construct
`\langif{it}{If vero: questo e' italiano.}{Else: this is for any language
different from Italian.}`
