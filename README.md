# Wikidata properties usage history
This repository contains data of historical usage statistics for Wikidata properties.
That it, it allows you to determine the number of usages of a property in various points of time in history.

## Data source
The data was extracted from the history of [Template:Property uses](https://www.wikidata.org/wiki/Template:Property_uses)
which has been automatically updated by a bot.
However, the data in this repository are limited to data prior to 2020-05-14, because on that day,
[the method of counting was changed](https://www.wikidata.org/wiki/Template_talk:Property_uses#Change_of_method).
Newer data for a selected subset of properties might be available under [Wikidata:Statistics/count/…](https://www.wikidata.org/wiki/Special:PrefixIndex/Wikidata:Statistics/count/P).

## Repository structure
The dataset is split to individual files containing just the number of usages of a single property on the given day (i.e. a JSON file containing _just_ the number),
on the path _year_/_month_/_day_/_property_`.json`, e.g. [`2019/11/25/691.json`](/2019/11/25/691.json) contains the number of usages
of the [P691 property](https://www.wikidata.org/wiki/Property:P691) on 2019-11-25.

Additionally, an index file for every year resides at _year_/`_index.json` (e.g. [`2019/_index.json`](/2019/_index.json), containing an index of all available
dates in the given year (because the data was not updated daily).

The raw data is directly accessible using the `raw.githubusercontent.com` URL, e.g. [the abovementioned `2019/11/25/691.json`](https://raw.githubusercontent.com/mormegil-cz/wdprop-usage-history/master/2019/11/25/691.json).

## License
All data in Wikidata is licensed under [CC-0](https://creativecommons.org/publicdomain/zero/1.0/). The [source page](https://www.wikidata.org/wiki/Template:Property_uses)
from which this repository was compiled, is, [strictly said](https://www.wikidata.org/wiki/Wikidata:Copyright),
under [the CC-BY-SA 3.0 Unported license](https://creativecommons.org/licenses/by-sa/3.0/). My contribution by compiling this repository is released under CC-0.

Therefore, the repository is available _at least_ under CC-BY-SA 3.0 Unported.
(You might believe the robotic compilation of the source page does not enjoy copyright/database right protection, in which case the data would be CC-0. Your call, I am not a lawyer.)
