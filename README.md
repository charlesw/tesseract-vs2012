Please note that this repo has now been superseeded by [tesseract-vs](https://github.com/charlesw/tesseract-vs).

tesseract-vs2013
================

Tesseract OCR engine dependencies with VS 2013 support, both 64 and 32 bit.

This repository contains the dependencies for Google's [Tesseract OCR project](https://github.com/tesseract-ocr/tesseract) for tesseract 3.04 and leptonica 1.74.1, along with dependencies for everything but WEBP support.

### Build Instructions

1. Open VS 2013 Developer Command Prompt and change the directory to this repository.
2. Execute the following command ``msbuild build.proj``

The build libraries and headers will be copied to ``~\release`` when done.

### Building tesseract

**Note:** The following assumes that your working directory is ``C:\tesseract-build\``, however this can be wherever you want.

1. Copy ``vs2013+64bit_support.patch`` to ``C:\tesseract-build\``
2. Checkout the tesseract source from [GIT Repo](https://github.com/tesseract-ocr/tesseract.git) into ``C:\tesseract-build\tesseract``.
3. Checkout the tesseract leptonica compile library source from [GIT Repo](https://github.com/bygreencn/tesseract-vs2013.git) into ``C:\tesseract-build\tesseract-lept``.
    ...
4. Copy the previously built dependencies to the parent directory (e.g. ``C:\tesseract-build\``)
5. Open the ``C:\tesseract-build\tesseract\vs2013\tesseract.sln`` solution in VS 2013 and build your desired configuration.

## License

All projects are made available under their original license(s).

* Leptonica - ``~/liblept/leptonica-license.txt``
* GifLib - ``~/giflib/COPYING``
* LibJpeg - ``~/libjpeg/README``
* LibPng - ``~/libpng/LICENSE``
* libtiff - ``~/libtiff/COPYRIGHT``
* libwebp - ``~/libwebp/COPYING``

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
