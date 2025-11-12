# FAQs

## What is SKOS?

The NERC Vocabulary Server (NVS) makes use of the World Wide Web Consortium's (W3C) Simple Knowledge Organization System (SKOS) to represent knowledge in a format understandable by computers. SKOS organises concepts into collections and schemes. These are further defined below.

## What is a concept?

A concept is an idea or notion; a unit of thought that can be clearly described. A concept is formally identified by a Unique Resource Identifier (URI), and can be connected to other concepts through relationships, known as mappings (more info below).

Example:  http://vocab.nerc.ac.uk/collection/L22/current/TOOL2179/ describes a specific dissolved oxygen sensor.

Example: http://vocab.nerc.ac.uk/collection/P01/current/DOXYZZ01/ describes the parameter measured by the dissolved oxygen sensor.

## What is a collection or controlled vocabulary?

Collections, also known as controlled vocabularies, are lists of unique concepts that are grouped by a common theme. Collections provide a convenient way to group concepts or place them in a meaningful order, under a common label. Collections are generally associated with a governance group who have the authority to create, deprecate or modify concepts within the collection. 

Example: http://vocab.nerc.ac.uk/collection/L22/current/

## What is a scheme?

A scheme is an aggregation or subset of unique concepts that are already registered in one or more existing collections, represented as a single semantic unit. Semantic relationships between concepts may also be viewed as part of the scheme.  

Example: http://vocab.nerc.ac.uk/scheme/OG_SENSORS/current/ is a scheme used by the OceanGliders community which groups a subset of existing concepts from the L22 collection into a single unit. The sensors relevant to their community are more easily found and accessed, as they need only search the subset, rather than the whole L22 collection.  

## What is a mapping?

A mapping is the established relationship between two concepts, collections or schemes. It is a way of linking these things together using a defined set of relationships or hierarchies, such as broadMatch, narrowMatch, relatedMatch, exactMatch.

Example: A concept for "mammals" in one collection might have skos:broadMatch to the concept for "animals" in another collection, showing that the "mammals" concept is a subset of "animals". 

## Summary of SKOS:

Using SKOS, concepts can be:
- Uniquely identified using Unique Resource Identifiers (URIs)
- Linked to other concepts through semantic relations
- Organised into informal hierarchies and association networks through: 
  - aggregation into concept schemes
  - grouping into labelled and/or ordered collections
  - mapping to concepts in other collections or schemes
 
## Why should I used controlled vocabularies for my dataset(s)?

For a scientific dataset for example, the metadata about what was measured, when, where, how, why and by who are all important pieces of information that provide the context surrounding the dataset. Individual concept URIs from various controlled vocabularies can be used in place of free text headings or attributes within data files, to ensure we are all talking the same language when describing a dataset.

The information described within a unique concept from a controlled vocabulary is organised in a standardised way, so that unabmiguous consistent meaning can be derived. The structure ensures the information is not only human-readable, but machine-readable, which is the key to enabling datasets from different sources to become comparable and interoperable.

An introduction to controlled vocabularies can be viewed here: https://youtu.be/kKOiPxq6E5M?t=112
