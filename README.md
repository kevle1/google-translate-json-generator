# Google Translate JSON Generator

A simple script to generate a JSON list of translations from Google Translate results

Used for my personal site to present greetings in various different languages. Could be used for any other text. **See hello.json** ☺

## Usage

`pip install -r requirements.txt`

`python translate.py -t hello`

### Optional parameters
`-s` Source language (ISO-639-1) (default `EN`)

`-o` Output filename (default `result.json`)

## Notes

The language to country mappings may not adequately represent all countries/ languages due to its subjectivity. Mappings based on: https://github.com/lipis/flag-icons/issues/510

Google Translate uses ISO-639-1 codes, hence the use of the mapping file instead of any library like [PyCountry](https://pypi.org/project/pycountry/) which uses ISO-639-3 values.

## Todo:

Dynamically load countries