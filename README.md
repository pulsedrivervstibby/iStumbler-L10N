# iStumbler-L10N
iStumbler Localization Files Public Repository - Fork, Translate and Send a Pull Request!

## Strings

iStumbler has a number of modules and plugins each with a seperate strings file, including various xib files, internal frameworks and plugins.

## Extracting Strings

ibtool can be used to extract strings from xib files

    // this works but isn't reccomended
    find . -name \*.xib | xargs -t -I '{}' ibtool --generate-strings-file '{}'_xib.strings '{}'

    // after property setting up the projects
    find . -name '*.strings' | cpio -pvdumB ../iStumbler-L10N/

    // TODO create a script to preview the changes in the running app

## License

    MIT License

    Copyright (c) 2018 Alf Watt & Localization Contributors

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.

