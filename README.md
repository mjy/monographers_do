# To answer the question "Monographer, what do you do?" I want others to to understand that "my" data are accessible to you already

## What is this?
This is a very hastily done brainstorm. As part of the [Revitalizing Monographs](https://revitalizingmonographs.org/) workshops various premises and thought experiments were raised that suggested that part of what needs to be done to "revitalize" monography is to point the broader community to tools, processes, and methods that _already exist_.  We don't mean to imply that things are "solved" in any of these areas. We do mean to imply that there are numerous, often very good, options out there for getting the core data in a Monograph into others hands/machines, and that some of these options adequately address requests being made of monographers. There are also emerging technologies that seek to serve Monographers explicitly that people may not be aware of.

This is an opinionated list.  It's trying to make a particular point (and raise others) rather than be comprehensive/correct etc.

The content here is gathered in such a format that it could, maybe, be summarized in a 5-6 minute lightning talk.

## Contributing 
You can contribute to this by either opening an issue or making a pull request. All errors, misinterpretations, etc. are Matt Yoder's fault, not the collaborating contributors. 

## Licence
CC 0. 

## Format
Each "My X" section/slide represents a type of data in a monograph and has up to three categories:
1) (Do) Now - You can do this now!
2) (Do) Soon - Sensu the Workshop's "I can imagine this technology existing already", _not_ "feature available tomorrow"
3) (To) do - Quick ideas/opinions/comments about missing bits.

TODO? - At the end of this section a series of hyperlinks reference the issues raised at the workshop as recorded on the "stickies" there.

# Presentation

## My team
### Now
Get an ORCID id, get your collaborators ORCIDs. Add ORCIDs to your data (e.g. in `recordedByID` or `identifiedByID`). Get a Wikidata Q id for your people, for dead people who collected the specimens you looked at. Spam these IDs everywhere you archive other data (e.g. Figshare, Zenodo, Publishers, all take ORCIDs now). Publish your data with ORCIDs to GBIF, watch people find your data by looking *you* up at GBIF.  You're a primary curator/producer, so Bionomia has less impact for you during production of the monograph, i.e. by definition you're re-examining specimens and their data, but when your data get to GBIF, then your data will be visible in platforms like Binomia, i.e. more accessible. Use tools like TaxonWorks to reference People as things, not rows of data while you compile your monograph.
### Soon
Publish your People to Wikidata via tools like TaxonWorks.
### Do

## My specimens
### Now 
Ensure your physical specimens have catalog numbers. Share your specimens with GBIF via DwC format. Pensoft will help do this. There are many other routes including publishing your dataset on Zenodo, Github, IPTs, etc. and pointing GBIF there. Numerous platforms exemplify tools that facilitate the pre-aggregation and curation of these data (e.g. Specify, TaxonWorks, Symbiota, Open Refine, Arctos). All of these data form the core of the "Digital Specimen".  You, as a monographer don't have to worry about that downstream job, just remember: 1) Catalog numbers on specimens; 2) Recommended bonus: UUIds for the occurrence going to GBIF as well. 
### Soon 
Better rendering of specimens in _human readable format_.
### Do
Relatively speaking this is very well worked out. 

## My Nomenclature
### Now 
Add your data to [Zoobank](http://zoobank.org/), Pensoft will do it all for you, you'll get LSIDs for names by doing this. You can do it yourself if you want. Or don't. Share your nomenclature to GBIF via a DwC Checklist. Share your nomenclature to the [Catalog of Life](https://www.catalogueoflife.org/) via _basically any format you want_ (assuming its a monograph with global coverage). Share your data to the World via the CoLDP format (TaxonWorks, WORMS, many others).  Share your ridiculously semantic [NOMEN](https://github.com/SpeciesFileGroup/nomen) referencing nomenclature via a public [TaxonWorks API](https://api.taxonworks.org/#/taxon_names).

## My phylogeny
### Now
Load your tree, pre-publication even, to [Open Tree](https://opentreeoflife.org).

## My biological relationships 
### Now
Just put some sort of table on a Github pages (or Google Drive, or anywhere that table is online) and whisper in the ear of [Globi](https://www.globalbioticinteractions.org/about), you're good.

## My descriptions
### Now
The text description. If it's published in Pensoft it's been processed by Plazi and isolatable via Pensoft and Plazis tools. You can also publish NeXML, Nexus, TNT, CSV versions of your data your companion Git repository. You can share your Observations (matrix, phylogenetic or descriptive) via a TaxonWorks JSON serving endpoint. You can do [crazy things like make Manchester syntax statements with rediculous OWL references](https://bioip.github.io/) (e.g. go to the lengths to produce RDF triples). You can use old tools like LUCID and others that will spit out SDD format. You could co-opt Mesquite or other matrix building software to manage your states in a matrix. You can use a simple script to compose your telegraphic sections (tools like 'mx', vSysLab, etc. have been doing this for over a decade, tools like IntKey have been doing this for decades). Create RC5/21 assertions between your taxa, share the corresponding CSV on your companion Git repository.
### Soon
More flash, not much more substance.
### Do
MorphDBase2 levels of instance based assertions.

## My DNA
### Now 
Scientists have been sending data to Genbank for a long time. Most importantly, you're a monographer and know that unique-identifier based vouchering, or the use of UUIDs when vouchering is not possible, is the foundation of your monograph, so you include references to those in your uploads whenever possible. You can also send your data to BOLD.
### Soon 
### Do 

## My Images
### Now
OK, this is awful. But wait- Zenodo, Figshare, Morphosource! Upload your plates. Get DOIs. Share all your images, and their metadata via a TaxonWorks API.
### Soon 
Cleverly point Internet Archive at your images.
### Do
Use IPFS peer-to-peer to share your images bit-torrent-esqe style.

## My archive
### Now
Did you know that [adding a repository to Github is perhaps the single best ultra long term archive of your data at the moment](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/about-archiving-content-and-data-on-github#about-the-github-archive-program)? Zip everything, compute a SHA for the zip, reference the SHA in your publication.  Put the Zip and the SHA "out there". Also, make crude webpages using free [Github pages](https://pages.github.com/), point the [Internet Archive](https://archive.org/index.php) at them.
### Soon
Tools like TaxonWorks could package your data from all the steps, sans images, and shove them on a Git repo or Publisher for you.
### Do
Git + images (or large genomic datasets) doesn't work so well.

## My anatomical insights
### Now
[Crossreference an OBO foundry ontology](https://obofoundry.org/). Contribute your data to a growing number of anatomical ontologies.  Get your vertebrate data in [Phenoscape's](https://phenoscape.org/) hands. Create a ["URI table" where possible](http://portal.hymao.org/projects/32/public/ontology/analyze).  Use ImageJ and other tools to auto-measure your anatomy and provide tables of data (e.g. Ants, Odontates, Fish) to your companion Git repo.
### Soon
Moaaar anatomy ontologies. Semantic labelling of images.
### Do

## Shameless plug
Does your monograph contain [stuff like this](https://stats.taxonworks.org/?server=sfg.taxonworks.org)? Then it can be [shared in places like this](https://api.taxonworks.org/). 
