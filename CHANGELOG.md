## 0.1.7 (2014-03-24)
* enhancement: @antoinepairet: Add support for `.scss` file extension
* development: Moved changelog to CHANGELOG.md
* development: @jasonsims: Added [TravisCI][travisci] integration
[travisci]: https://travis-ci.org/niftylettuce/node-email-templates

## 0.1.6 (2014-03-14)
* development: @jasonsims: Deprecated windows branch and module

## 0.1.5 (2014-03-13)
* bugfix: @miguelmota: Batch templateName issue

## 0.1.4 (2014-03-10)
* bugfix: Misc bugfixes to main
* development: @jasonsims: Abstracted templateManager
* development: @jasonsims: Added integration tests
* development: @jasonsims: Added unit tests

## 0.1.3 (2014-03-03)
* enhancement: @jasonsims: Added support for various CSS pre-processors

## 0.1.2 (2014-02-22)
* enhancement: @jasonsims: Added support for multiple HTML template engines

## 0.1.1 (2013-12-14)
* bugfix: Long path issue for Windows

## 0.1.0 (2013-04-16)
* bugfix: Batch documentation issue

## 0.0.9
* bugfix: Juice dependency issue

## 0.0.8 (2013-03-03)
* enhancement: Minor updates

## 0.0.7
* enhancement: @nicjansma: Added support for ejs's include directive

## 0.0.6 (2012-11-01)
* bugfix: @vekexasia: Fixed batch problem (...has no method slice)

## 0.0.5 (2012-09-12)
* enhancement: Added support for an optional zlib compression type. You can
  now return compressed html/text buffer for db storage

  ```javascript
  template('newsletter', locals, 'deflateRaw', function(err, html, text) {
    // The `html` and `text` are buffers compressed using zlib.deflateRaw
    // <http://nodejs.org/docs/latest/api/zlib.html#zlib_zlib_deflateraw_buf_callback>
    // **NOTE**: You could also pass 'deflate' or 'gzip' if necessary, and it works with batch rendering as well
  })
  ```

## 0.0.4
* enhancement: Removed requirement for style.css and text.ejs files with
  compatibility in node v0.6.x to v0.8.x. It now utilizes path.exists instead
  of fs.exists respectively.