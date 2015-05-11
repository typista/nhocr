Since Sep 8, 2008 / Last update: Aug 30, 2014

# Introduction #
NHocr is a command line OCR (Optical Character Recognition) program for Japanese language, etc. It has been designed to recognize machine-printed Japanese characters and some ASCII characters/symbols in an image.
NHocr is probably the first Open Source Japanese OCR software (offline, machine-printed), except some experimental, partial codes open to academic communities.

You can also use NHocr through WeOCR service at:
  * http://maggie.ocrgrid.org/nhocr/

The program is highly experimental, and the character recognition performance is limited. (You would become happier with a commercial product if you want a high performance OCR.)

The character feature used in NHocr is based on Peripheral Local Moment (P-LM) proposed by Hori et al. in late 90's.

NHocr is originally a product of the author's weekend programming. The development work may be rather slow.

# Change of the source package repository (important) #

The source package repository has been changed to SourceForge.JP
since Google removed "Downloads" feature at Google Code.
The conventional tar-ball distribution is preferred in this project.
This project page remains so you can find older versions.

The newer NHocr packages and supporting materials can be found at:
  * https://sourceforge.jp/projects/nhocr/

# Limitations of the current version #

  * The current NHocr can handle text block image only, since it has not been equipped with a page layout analysis engine.
  * The recognition accuracy may deteriorate when wide and narrow characters are mixed or when proportional fonts are used.
  * The character segmentation performance is limited, since a primitive segmentation algorithm is used in the current version.
  * The recognition accuracy with ASCII characters may not be so good. Using another OCR, such as tesseract, is recommended for European languages.
  * The language post-processor "gramd" is experimental and works with Japanese text only. Some side effects may exist.



# Supported platforms and requirements #
Solaris SPARC/x86 and Linux are officially supported.
NHocr would work on other UNIX(-like) platforms and MS-Windows.

NHocr uses FreeType 2 available at:
  * http://www.freetype.org/

NHocr 0.21 and older depend on O2-tools package available at:
  * http://www.imglab.org/p/O2/

# Supported languages #
The current version of NHocr supports Japanese only.

The author is interested in supporting other oriental languages such as Chinese. Character code table cctable-xxx is required. Contributions are welcome.

# License #
Apache License 2.0 applies to newer versions.

A derivative of MIT-X applies to version 1.5e-32 and older.