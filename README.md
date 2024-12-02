# Accellera Documentation Flow (ADF)

The Accellera Documentation Flow offers the infrastructure to develop and publish Accellera (Draft) Standards, User Guides and other standard-related documentation. The main output are high-quality documents in Portable Document Format (PDF) compliant with the IEEE SA Standards Style Manual. Future extensions of this flow will also render interactive browser-compatible standards in HTML format. 

The documentation flow is documented in the Accellera Style Guide, which explains the Markdown formatting and styles to create IEEE SA Standards compliant documents.

## Usage

The document sources shall be located in directory `books/<standard-document>/`.

The document metadata (e.g. properties) shall be located in directory `_data/works/<standard-document>/`.

To render a PDF document using the Accellera Documentation Flow, use the following command:

```sh
$ npm run eb -- output --format screen-pdf --book <standard-document>
```

It will generate a PDF document in the `_output` directory.

Please contact the Technical Committee Chair in case of questions on the Accellera Documentation Flow, the required installation procedure or use of the standard document templates.

## Acknowledgment

Special thanks to [Electric Book Works](https://electricbookworks.com/) for the development and support of the Accellera Documentation Flow.
