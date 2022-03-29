# Scripts to enrich VOC datasets

This repo contains two scripts (Python/Jupyter) to enrich the data from three different datasets on the shipping of the Dutch East India Company (VOC) by linking them together. The main goal is to get a list of disambiguated ships and create links from that list to the three sets.

The datasets involved are:

#### Dutch-Asiatic Shipping in the 17th and 18th centuries (DAS)

<a href="http://resources.huygens.knaw.nl/das">DAS</a> is a dataset containing information on more than 4,700 voyages of the VOC. The set is limited to intercontinental voyages between Europe and Asia. Importantly, it contains a disambiguated list of ships. 

#### Bookkeeper-General Batavia (BGB)

<a href="https://bgb.huygens.knaw.nl/">BGB</a> is a dataset with information on almost 20,000 voyages of the Dutch East India Company (VOC), which includes information on cargoes carried and ship used. It does not contain a disambiguated list of ships, i.e. a single ship name may refer to multiple physical vessels.

#### Generale Zeemonsterrollen (GZM)

<a href="https://maritiemportal.nl/generale-zeemonsterrollen-voc-1691-1791-huygens-ing/">GZM</a> is a dataset with information on more than 5,300 musterings done in the late seventeenth and eighteenth century by officials of the Dutch East India Company (VOC). In a mustering, all personnel serving on a vessel or land-based location were listed. For vessel musterings, the dataset includes standardized versions of the ship names. There is no disambiguated list of shipnames, i.e. a single ship name may refer to multiple physical vessels in the dataset.

***

## Scripts

The first script, <a href="https://github.com/GdeCook/enrich_from_das/blob/8c3ebb33dcacb85ea93c80115b148a577d95d693/BGB-voyages%20to%20DAS%20ship%20IDs.ipynb">BGB-voyages to DAS ship IDs.ipynb</a>, establishes a link between (unique) shipvoyage IDs in BGB and DAS ship IDs. The second script, <a href="https://github.com/GdeCook/enrich_from_das/blob/8c3ebb33dcacb85ea93c80115b148a577d95d693/Remaining%20BGB%20and%20GZM%20ships.ipynb">Remaining BGB and GZM ships.ipynb</a>, links GZM musterings to DAS ships IDs. In addition, it distills a list of unique ships that are not present in DAS, gives these ships unique IDs and creates links between those IDs and GZM and BGB. Further details are available inside each script.
