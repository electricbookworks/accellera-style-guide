# CCI documentation

## LRM authoring

The sources of the CCI Language Reference Manual can be found in the `cci/` directory. Use your favorite editor make make any changes to the document sources.

## LRM PDF document generation

To render the CCI Language Reference Manual as PDF document, the Accellera documentation flow is required. More information can be found in the [tc-documentation](https://github.com/OSCI-WG/tc-documentation/) repository.

After installation of the Accellera documentation flow, use the following command to create the PDF:

```sh
npm run eb -- output --format screen-pdf --book cci
```

It will generate a PDF in the `_output` directory.

## Questions and support

Please contact the Technical Committee chair in case of questions on the Accellera documentation flow, the required installation procedure or use of the standard document templates.
