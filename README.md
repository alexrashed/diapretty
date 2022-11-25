# diapretty - LocalStack diagnosis pretty printer

Users of [LocalStack](https://github.com/localstack/localstack) can create diagnostics reports via the diagnostics endpoint:

```shell
curl -s localhost:4566/_localstack/diagnose | gzip -cf > diagnose.json.gz
```

This report contains a lot of data, which can be a bit overwhelming. 

`diapretty` helps with that, by taking all the data from the report and putting it into a nice to read HTML report which is automatically opened in your browser.

# Installation

Just do `pip install -e .` in this directory

# Usage

After installation, you can use diapretty like this:
```shell
python -m diapretty.main /path/to/diagnose.json.gz
```

Enjoy!