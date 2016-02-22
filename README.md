# Taxonomic Classification of Images using ANNs

Naturalis Biodiversity Center has an ongoing interest in the development of methods for
automated image recognition and taxonomic classification. This repository aggregates the
work that has been done (led by @rvosa) to do this in such a way that:
- a generic framework develops that can be applied to a variety of different cases. So
  far these consist of the classification of slipper orchids, and of Javanese butterflies.
  However, other cases ought to be possible as well.
- no specific assumptions about, for example, landmarks or other prior knowledge about
  morphology are necessary. Hence image features should be quite generic, although we
  should be able to choose among generic features to select the ones that perform best
  on any given case.
- the taxonomic classification can be approximated if not fully determined. For example,
  it would be useful if an image could at least be classified to the genus level if not
  the species.
- the framework can be presented in a user-friendly way, which includes appropriate 
  presentation and user experience on mobile platforms.

## Project structure

The current repository aggregates projects related to image classification. Contains 
relevant [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules).

![Project structure](structure.png)

## Explanation of submodules

### Currently under active development

The following submodules are currently (February 2016) under active development and/or
are expected to receive additional commits

- [imgpheno](https://github.com/naturalis/imgpheno) - general purpose python library for 
  image segmentation and feature extraction.
- [nbclassify](https://github.com/naturalis/nbclassify) - image classification framework,
  includes interaction with Flickr, with ANNs, and OrchID web application
- [nbclassify-data](https://github.com/naturalis/nbclassify-data) - data repository for
  image metadata, extracted image features, and FANN neural networks.

### Potentially useful but not under active development

The following submodules contain code that is potentially useful at time of writing (February
2016) but is not intended to undergo additional development.

- [ai-fann-evolving](https://github.com/naturalis/ai-fann-evolving) - a genetic algorithm that
  evolves optimal parameterization of ANNs. Written in Perl, as `AI::FANN::Evolving`. Not under 
  active development, ignore.
- [puppet-orchid](https://github.com/naturalis/puppet-orchid) - provisioninf scripts to configure
  a web server for OrchID web application. Not under active development, ignore.

### Only here for archival purposes

The following submodules are here for archival purposes because they were presentational
milestones earlier in the project.

- [orchid-presentation](https://github.com/figure002/orchid-presentation) - LaTeX sources to
 generate orchid classification slides. Only here for archival purposes, ignore.
- [orchid-report](https://github.com/naturalis/orchid-report) - LaTeX sources to generate 
  orchid classification report. Only here for archival purposes, ignore.
- [img-classify](https://github.com/rvosa/img-classify) - proof-of-principle to show how ANNs
  can discriminate between beetles and butterflies. Only here for archival purposes, ignore.
