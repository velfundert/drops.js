# Drops.js &ndash; Multiple file upload with drag and drop

Drops.js is a utility library for performing multiple file upload over ajax using drag and drop.

## Usage

```javascript
/*
 * Create a new dropzone for uploading files.
 *
 * @selector: The DOM file drop zone. Must be present in the DOM when drops() is called.
 * @options: An object with parameters, modifiers and callbacks (see below).
 */
drops(selector, options);
```

## Options

Parameters:

* **url**: The server address that receives the upload (default "/").
* **field**: The name of the file field in each request (default "file").
* **method**: The HTTP method for each upload (default "POST").
* **accept**: The expected return type from the server (default "text").

Modifiers:

* **formData**: Function to augment or change the formData object.
* **xhr**: Function to augment or change the XHR object.

Upload callbacks:

* **progress**: Handler called on progress events, for each file.
* **error**: Handler called on errors, for each file.
* **success**: Handler called when each file is uploaded.
* **complete**: Handler called when all files are uploaded.

Event callbacks:

* **dragenter**: Handler called on "dragenter".
* **dragover**: Handler called on "dragover".
* **dragexit**: Handler called on "dragexit".
* **dragleave**: Handler called on "dragleave".
* **dragend**: Handler called on "dragend".
* **drop**: Handler called on "drop".

## License

MIT. See LICENSE.
