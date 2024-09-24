# Python Documentation Editorial Board

This repo contains activity updates, process, and planning information for the Python Documentation Editorial Board.

See [PEP 732](https://peps.python.org/pep-0732/).

## Changelog

We have a "changelog" of decisions: [CHANGELOG.md](CHANGELOG.md). 

## Updates

[Read updates](https://python.github.io/editorial-board/updates/) of the Editorial Board's activities.
Subscribe to the updates using the [RSS feed](https://python.github.io/editorial-board/updates/index.xml).

## Process

The Editorial Board's private meetings are monthly on the second Monday at 1:30pm Pacific.

If you have a general request or question, please use the [Documentation category in Discourse](https://discuss.python.org/c/documentation/26).

If you need Editorial Board assistance, please [file an issue on this repo](https://github.com/python/editorial-board/issues/new/choose).

## Reference

These links give context on the editorial board:
- [PEP 732](https://peps.python.org/pep-0732/)
- [PEP 732 Discourse discussion](https://discuss.python.org/t/pep-732-the-python-documentation-editorial-board/36710)
- [Language Summit 2021 presentation](https://pyfound.blogspot.com/2021/05/the-2021-python-language-summit-python.html)
- [Language Summit 2020 presentation](https://pyfound.blogspot.com/2020/04/cpython-documentation-next-5-years.html)

These links give context on existing documentation landing pages:
- [CPython Documentation Landing page (docs.python.org)](https://docs.python.org)
- [PSF (python.org) website landing page](https://python.org)
- [Documentation Experience presentation - Review navigation of PSF website related to docs](https://docs.google.com/presentation/d/1ujDv8wViPvAMFAtYCRxSKh-CMUlbjcfVYitsqEI2Ios)


## Writing new content

Hugo is not needed to be installed in order to write a new meeting minutes.

Write the meeting minutes a markdown file under ``content/updates/*.md``, commit, and
create the pull request. A preview will then be generated on Netlify.

The meeting minutes should be written using template provided in [archetypes/updates.md](/archetypes/updates.md).

If you have Hugo installed, a new meeting minutes file can be created by typing on the command line:

```
hugo new content content/updates/newupdate.md
```

This will create the file under ``content/updates/newupdate.md``, and you can continue editing it.

(replace "newupdate.md" with the desired filename.)

## Building the static site locally

1. First install Hugo.

2. Run the command at the root of the repository:

```
hugo server
```

## Writing new changelog

Use the template in [archetypes/changelog.md](archetypes/changelog.md).

The file can also be created using the command:

```
hugo new content content/changelog/newchangelog.md
```

It will create a new file under ``content/changelog/newchangelog.md``. (Replace "newchangelog.md" with the desired filename).