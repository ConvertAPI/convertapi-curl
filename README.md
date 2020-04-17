## Simple conversion methods

Web to PDF API https://www.convertapi.com/web-to-pdf

```nginx
curl -F "Url=https://www.google.com" -F "StoreFile=true" https://v2.convertapi.com/convert/web/to/pdf?Secret=your-api-secret
```

Excel to PDF API https://www.convertapi.com/xlsx-to-pdf

```nginx
curl -F "File=@/path/to/doc.xlsx" -F "StoreFile=true" https://v2.convertapi.com/convert/xlsx/to/pdf?Secret=your-api-secret
```

Remote Word to PDF API https://www.convertapi.com/docx-to-pdf

```nginx
curl -F "File=https://cdn.convertapi.com/cara/testfiles/document.docx" -F "StoreFile=true" https://v2.convertapi.com/convert/docx/to/pdf?Secret=your-api-secret
```

## Convert a local file

Word to PDF API https://www.convertapi.com/xlsx-to-pdf

```nginx
curl -F "File=@/path/to/doc.docx" -F "StoreFile=true" https://v2.convertapi.com/convert/xlsx/to/pdf?Secret=your-api-secret
```

## Convert a remote file and set additional parameters

Set input and output formats and pass file parameter.

PowerPoint to PNG API. Read more https://www.convertapi.com/pptx-to-png

```nginx
curl -F "File=@/path/to/presentation.pptx" -F "StoreFile=true" -F "ImageResolutionH=500" -F "ImageResolutionV=500" -F "ScaleImage=true" -F "ScaleProportions=true" https://v2.convertapi.com/convert/pptx/to/png?Secret=your-api-secret
```

## Read the account status

Get infomration about your user account

```nginx
curl https://v2.convertapi.com/user?Secret=your-api-secret
```

## Supported file formats, conversions and actions

https://www.convertapi.com/doc/supported-formats
