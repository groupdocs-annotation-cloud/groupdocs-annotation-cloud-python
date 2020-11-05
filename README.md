![](https://img.shields.io/badge/api-v2.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/groupdocs-annotation-cloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/groupdocs-annotation-cloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/groupdocs-annotation-cloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/groupdocs-annotation-cloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/groupdocs-annotation-cloud) ![PyPI - Status](https://img.shields.io/pypi/status/groupdocs-annotation-cloud) [![GitHub license](https://img.shields.io/github/license/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python)](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python/blob/master/LICENSE) 

# Annotate Documents via Python

[GroupDocs.Annotation Cloud SDK for Python](https://products.groupdocs.cloud/annotation/python) wraps GroupDocs.Annotation RESTful APIs so you may integrate Document Annotation features in your own apps with zero initial cost.

The solution helps in applying annotations, sticky notes, watermark overlays, redactions, text replacements and markups to documents, presentations, emails, spreadsheets, PDF, images, and other file formats.

## Annotate Documents & Images in the Cloud

- Import document annotations.
- Add or remove annotations.
- Export annotated document back to its original format.
- Preview document pages as images.
- Fetch document information, such as, page count & file size.

Check out the [Developer's Guide](https://docs.groupdocs.cloud/annotation/developer-guide/) to know more about GroupDocs.Annotation REST API.

## Microsoft Office Formats

**Microsoft Word:** DOC, DOCM, DOCX, DOT, DOTM, DOTX, RTF\
**Microsoft Excel:** XLS, XLSX\
**Microsoft PowerPoint:** PPT, PPTX, PPSX\
**Microsoft Visio:** VSSX, VSS, VSSM, VDX, VSD, VSDX, VSDM, VSTM, VSX, VTX\
**Microsoft Outlook:** EML, EMLX, MSG

## Other Document Formats

**Portable:** PDF\
**OpenDocument:** ODT, OTT, ODP, OTP\
**Images:** BMP, PNG, JPG, JPEG, TIFF, TIF, GIF\
**Web:** MHTML\
**Others:** TXT

## Get Started with GroupDocs.Annotation Cloud SDK for Python

First create an account at [GroupDocs for Cloud](https://dashboard.groupdocs.cloud/) and get your application information. Next, follow the installation steps to get started.

### Installation

GroupDocs.Annotation Cloud SDK for Python is available at [PyPI](https://pypi.org/project/groupdocs-annotation-cloud/) so install it using [PIP](https://pypi.org/project/pip/) as follows.

```sh
pip install groupdocs-annotation-cloud
```

Or clone repository and install it via [Setuptools](http://pypi.python.org/pypi/setuptools):

```sh
python setup.py install
```

## Get Supported File Formats for Annotation

Please follow the [installation procedure](#installation) and then run following:

```python
# Import module
import groupdocs_annotation_cloud

# Get your app_sid and app_key at https://dashboard.groupdocs.cloud (free registration is required).
app_sid = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
app_key = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"

# Create instance of the API
api = groupdocs_annotation_cloud.InfoApi.from_keys(app_sid, app_key)

try:
    # Retrieve supported file-formats
    response = api.get_supported_file_formats()

    # Print out supported file-formats
    print("Supported file-formats:")
    for format in response.formats:
        print('{0} ({1})'.format(format.file_format, format.extension))
except groupdocs_annotation_cloud.ApiException as e:
    print("Exception when calling get_supported_file_formats: {0}".format(e.message))
```

## GroupDocs.Annotation Cloud SDKs in Popular Languages

| .NET | Java | PHP | Python | Ruby | Node.js |
|---|---|---|---|---|---|
| [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-dotnet) | [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-java) | [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-php) | [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python) | [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-ruby)  | [GitHub](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-node) |
| [NuGet](https://www.nuget.org/packages/GroupDocs.Annotation-Cloud/) | [Maven](https://repository.groupdocs.cloud/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation-cloud) | [Composer](https://packagist.org/packages/groupdocscloud/groupdocs-annotation-cloud) | [PIP](https://pypi.org/project/groupdocs-annotation-cloud/) | [GEM](https://rubygems.org/gems/groupdocs_annotation_cloud)  | [NPM](https://www.npmjs.com/package/groupdocs-annotation-cloud) | 

[Home](https://www.groupdocs.cloud/) | [Product Page](https://products.groupdocs.cloud/annotation/python) | [Documentation](https://docs.groupdocs.cloud/annotation/) | [Live Demo](https://products.groupdocs.app/annotation/total) | [API Reference](https://apireference.groupdocs.cloud/annotation/) | [Code Samples](https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-python-samples) | [Blog](https://blog.groupdocs.cloud/category/annotation/) | [Free Support](https://forum.groupdocs.cloud/c/annotation) | [Free Trial](https://dashboard.groupdocs.cloud)
