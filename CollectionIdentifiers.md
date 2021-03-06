# USI Collection Identifiers

The Universal Spectrum Identifier (USI) for Mass Spectrometry has as its second field a collection identifier.
The specification itself does not prescribe the complete list of allowable collection identifiers. Rather,
the list is maintained here at GitHub and is extensible in an open manner without changing the specification.

# Permitted Collection Identifiers:

1. PXDnnnnnn - The preferred collection identifier is of the form PXDnnnnnn, such as PXD017269
(http://proteomecentral.proteomexchange.org/dataset/PXD017269). The PXDnnnnnn SHOULD be used for all proteomics
mass spectrometry datasets that have been registered at ProteomeXchange.

2. MSVnnnnnnnnn - A collection identifier for datasets contained at the MassIVE repsository, such as MSV000078556. This type of 
identifier SHOULD only be used when there is not a corresponding PXDnnnnnn identifier for the dataset, as is often the case
for metabolomics datasets.

3. RPXDnnnnnn - A ProteomeXchange identifier for a reprocessed dataset of the form RPXDnnnnnn, such as RPXD006668
(http://proteomecentral.proteomexchange.org/dataset/RPXD006668). The RPXDnnnnnn SHOULD ONLY be used when there is no
corresponding PXDnnnnnn identifier available (as in the case where an RPXDnnnnnn dataset derives from a non-ProteomeXchange
dataset) or in the context of a PSM identifier

4. RMSVnnnnnnnnn - A collection identifier for reprocessed datasets contained at the MassIVE repsository, such as RMSV000078556.
This type of 
identifier SHOULD ONLY be used when there is not a corresponding PXDnnnnnn identifier for the dataset, since PXDnnnnnn identifiers are preferred.

5. USI000000 - A collection identifier to be used as a placeholder for an as-yet unknown collection identifier.
In cases where a USI must be written at a time when the final collection identifier is not yet known, 
a placeholder of USI000000 SHOULD be used, so as to enable a straightforward search and replace when the final PXD number
or other collection identifier is registered. Software implementations should recognize this string as a placeholder that needs to be resolved.

6. PXLnnnnnn - A ProteomeXchange spectral library identifier of the form PXLnnnnnn. All spectral libraries registered
through ProteomeCentral are given a PXLnnnnnn identifier. These collections contain representative spectra often aggregated
from several replicates, rather than original scan events in MS datasets as denoted by PXDnnnnnn identifiers.

There are no other approved collection identifiers at this time.

