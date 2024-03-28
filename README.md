# issuuzu

Quick capture tool for PDFs published on ISSUU.

## Usage

```
./isuuzu <url>
```

Where `<url>` is a page with one or more embedded ISSUU publications.

## Example

```
$ ./issuuzu https://www.botanicgardens.org.au/our-science/our-collections/botanical-illustration/the-florilegium-society
Fetching URL 'https://www.botanicgardens.org.au/our-science/our-collections/botanical-illustration/the-florilegium-society'
Found 2 publications.
Publication #1 of 2 total is at https://e.issuu.com/embed.html?backgroundColor=%23ffffff&backgroundColorFullscreen=%23ffffff&d=florilegium_cover_internals_issuu_ed_2023_1_&hideIssuuLogo=true&hideShareButton=true&u=royalbotanicgardensanddomaintrust"
Downloading publication at https://e.issuu.com/embed.html?backgroundColor=%23ffffff&backgroundColorFullscreen=%23ffffff&d=florilegium_cover_internals_issuu_ed_2023_1_&hideIssuuLogo=true&hideShareButton=true&u=royalbotanicgardensanddomaintrust"
 - User ID is royalbotanicgardensanddomaintrust
 - Data ID is florilegium_cover_internals_issuu_ed_2023_1_
Fetching matching embedded URL... OK
Fetching URL: https://reader3.isu.pub/royalbotanicgardensanddomaintrust/florilegium_cover_internals_issuu_ed_2023_1_/reader3_4.json
Downloading 228 pages....................................................................................................................................................................................................................................... done.
Converting to PDF ... florilegium_cover_internals_issuu_ed_2023_1_.pdf
Cleaning up single page image files ... done.
Publication #2 of 2 total is at https://e.issuu.com/embed.html?backgroundColor=%23ffffff&backgroundColorFullscreen=%23ffffff&d=botendvr_cover_internals_issuu_ed_2023_1_&hideIssuuLogo=true&hideShareButton=true&u=royalbotanicgardensanddomaintrust"
Downloading publication at https://e.issuu.com/embed.html?backgroundColor=%23ffffff&backgroundColorFullscreen=%23ffffff&d=botendvr_cover_internals_issuu_ed_2023_1_&hideIssuuLogo=true&hideShareButton=true&u=royalbotanicgardensanddomaintrust"
 - User ID is royalbotanicgardensanddomaintrust
 - Data ID is botendvr_cover_internals_issuu_ed_2023_1_
Fetching matching embedded URL... OK
Fetching URL: https://reader3.isu.pub/royalbotanicgardensanddomaintrust/botendvr_cover_internals_issuu_ed_2023_1_/reader3_4.json
Downloading 136 pages........................................................................................................................................... done.
Converting to PDF ... botendvr_cover_internals_issuu_ed_2023_1_.pdf
Cleaning up single page image files ... done.
$
```

## Requirements

 * `curl`
 * ImageMagick `convert` (to generate final PDF)

## Warranty

None.
