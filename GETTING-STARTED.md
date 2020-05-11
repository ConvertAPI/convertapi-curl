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

## Conversion chaining using cURL

Convert a PDF file into multiple JPG images and ZIP the converted result into a single archive on our server.

PDF to JPG API. Read more https://www.convertapi.com/pdf-to-jpg

```nginx
curl -F "File=@/path/to/document.pdf" -F "ImageResolutionH=500" -F "ImageResolutionV=500" -F "ScaleImage=true" https://v2.convertapi.com/convert/pdf/to/jpg?Secret=your-api-secret -F "StoreFile=true"
```

In this example we used a PDF document that consists of 3 pages which results in 3 separate JPG images. Now let's zip multiple converted files into a single archive.

JPG to ZIP API. Read more https://www.convertapi.com/jpg-to-zip

```nginx
curl -F "Files[0]=https://v2.convertapi.com/d/dda2ab19d23e7aaa4203b5ff1fa5a13b/document.jpg" -F "Files[1]=https://v2.convertapi.com/d/600e09f511ee90bbe5385ba32d791768/document-2.jpg" -F "Files[2]=https://v2.convertapi.com/d/8601b3e1ce2abad484cc58ef0c8f2a28/document-3.jpg" https://v2.convertapi.com/convert/jpg/to/zip?Secret=your-api-secret -F "StoreFile=true"
```

## Read the account status

Get infomration about your user account

```nginx
curl https://v2.convertapi.com/user?Secret=your-api-secret
```

## Supported file formats, conversions and actions

https://www.convertapi.com/doc/supported-formats
