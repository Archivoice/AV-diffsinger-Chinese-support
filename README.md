# AV-style-diffsinger-Chinese-system
A more detailed phonetic system for diffsinger Chinese

## [View phoneme chart](/Phonemes.md)

## [View dictionary](/dsdict)

The [dictionary-zh.txt](/dictionary-zh.txt) is a minimal dictionary for training, will not work with OpenUtau or command-line interface (CLI) inference.
For use in OU, use the dictionary provided [here](/dsdict), and for CLI inference, use [this](/dict-cn-CLI.txt).

## NNSVS 0.3.0 Chinese Phoneme Compatibility

The 0.3.0 version of our [Chinese support for NNSVS](https://github.com/Archivoice/nnsvs-chinese-support) does not have `i0` independent of `I`. And thus to fix issues with porting datasets labeled with that phoneme system, a regex string is provided below to batch replace the phonemes in the .lab files. The regex string will convert every instance of individual `I`, ie. `c I` => `c i0`.

Find:
```
(\d+ )I(|\n|\r)(\d+ \d+ (?!N|ng))
```
Replace:
```
$1i0$2$3
```
