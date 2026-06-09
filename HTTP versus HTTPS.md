# HTTP versus HTTPS

The distinction between `HTTP` and `HTTPS` is related to the distinction between a URI (Uniform Resource Identifier) and a URL (Uniform Resource Locator). A URI identifies a resource, whereas a URL describes how to access that resource. 

For example:

URI: http://vocab.nerc.ac.uk/collection/P01/current/TEMPPR01/

URL: https://vocab.nerc.ac.uk/collection/P01/current/TEMPPR01/

Both refer to the same concept, but the `HTTPS` URL describes the current secure access method.

## Why use URIs?

When recording identifiers in metadata, databases, or data products, use the URI provided by the authority that manages the resource. A URI is intended to remain stable over time, even if access protocols change or additional security measures are introduced. This helps maintain interoperability and ensures that references remain consistent across systems. 

## Why do some URIs use HTTP rather than HTTPS?

NERC Vocabulary Server (NVS) concept URIs use `HTTP` rather than `HTTPS` for historical and persistence reasons. The NVS was established before `HTTPS` became the standard for web traffic, and the existing `HTTP` URIs have been widely adopted in datasets, vocabularies, applications, and publications. Since URIs are intended to be stable, permanent identifiers, changing them would risk breaking existing references and reduce interoperability. 

This approach is common across the semantic web community; many well-established vocabularies and ontologies, such as Dublin Core and SKOS, continue to use `HTTP`-based namespace URIs while serving their content securely over `HTTPS`.

## Recommendation

The key point is that a URI should be treated as a persistent identifier, while a URL represents a particular way of retrieving the resource.
When recording a controlled vocabulary term or other persistent identifier, use the URI supplied by the authoritative source. Systems and web browsers can then resolve that identifier using the most appropriate access method.
Note: trailing slashes are part of every concept and collection in the NVS, as hierarchies and versioning are included in the URIs (e.g. http://vocab.nerc.ac.uk/collection/OG1/current/DPAR/1/ for version 1 of the concept). Users are therefore advised to use the trailing slash when referencing concepts or collections (e.g. http://vocab.nerc.ac.uk/collection/P01/current/ or http://vocab.nerc.ac.uk/collection/P01/current/TEMPPR01/).
