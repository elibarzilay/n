
# n

 My own flavour of node binary management, no subshells, no profile setup, no convoluted api, just _simple_.

## Installation

    $ npm install n

or

    $ make install

## Examples

Install a few nodes:

    $ n 0.2.6
    $ n 0.3.3

List installed nodes:

    $ n
    
      0.2.5
    * 0.2.6
      0.3.3

Pass some config flags to _./configure_:

    $ n 0.2.6 --debug --oprofile

## Usage

 Output from `n --help`:

     Usage: n [options] <version> [config]

     Commands:

       n               Output versions installed
       n <version>     Install and/or use node <version>

     Options:

       -V, --version   Output current version of n
       -h, --help      Display help information

## Details

 `n` by default installs node to _/usr/local/n/versions_, from
 which it can see what you have currently installed, and activate previously installed versions of node when `n <version>` is invoked again.

 Activated nodes are then installed to the prefix _/usr/local_, which of course may be altered via the __PREFIX__ environment variable.

 To alter where `n` operates simply export __N_PREFIX__ to whatever you prefer.

## License 

(The MIT License)

Copyright (c) 2010 TJ Holowaychuk &lt;tj@vision-media.ca&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.