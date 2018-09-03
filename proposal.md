# PIDS in Dublin Core - Proposal

## Context

The exchange of metadata between systems involved in scholarly publishing (and Open Access) is a key activity in that domain. Metadata from repositories is typically 'batch-harvested' using an HTTP and XML based protocol, [OAI-PMH](https://www.openarchives.org/OAI/openarchivesprotocol.html). In this context, repositories (and related systems) make much use of the DCES in a number of application profiles (e.g.  [OAI_DC](https://www.openarchives.org/OAI/openarchivesprotocol.html),  [OpenAIRE v4 (in beta)](http://openaire-guidelines-for-literature-repository-managers.readthedocs.io/en/latest/application_profile.html), [RIOXX v2](http://www.rioxx.net/profiles/v2-0-final/) etc.). OAI_DC is the default application profile used by OAI-PMH and is composed entirely of properties from the DCES.

Within this domain there is growing interest in the use of global persistent identifiers (PIDs) and a realisation that, without them, metadata is considerably less useful. The inclusion of PIDs in such metadata is somewhat arbitrary - many metadata records will contain one PID - identifying the subject of the record - but are less likely to contain any others, despite the record referencing identifiable resources (authors, organisations, other resources etc.)

For a majority of cases in this domain, the most important resources to be identified with PIDs are:

* scholarly outputs (e.g publications, research data, software sources etc.) which are generally identified with either a DOI (in HTTP URI form) or with a general URL.
* authors and contributors - while several schemes are in use, ORCID is becoming recognised as the conventional identifier agency and format for these, providing ORCID IDs (also in HTTP URI form)
* Organisations - especially funders, and also institutions with which authors are affiliated.

## Project description

This initiative seeks to develop a DCMI recommendation on how to express Persistent Identifiers (PIDs) in XML-based metadata application profiles which use properties from either the [Dublin Core Metadata Element Set](http://www.dublincore.org/documents/dces/) (DCES) or the [DCMI Metadata Terms](http://www.dublincore.org/documents/dcmi-terms/).

This recommendation should have wide applicability. It is required in particular by several organisations working in the general domain of scholarly communications, and with open-access repository systems in particular. This work will, therefore, benefit from the focus provided by some closely related 'real world' user-stories.

This project will:

1. Solicit 'real-world' user-stories and use-cases from interested parties, using the 'issues' feature in this repository.
2. Develop some candidate approaches to expressing PIDs in metadata using properties from the Dublin Core vocabularies in the context of the examples described in #1.
3. Hold a special session at the [DCMI annual conference in Porto, Portugal in September 2018](http://www.dublincore.org/conference/2018/), where the candidate approaches will be discussed with the intention of agreeing a consensus.
4. Publish the results, either as a DCMI Recommendation or as a revision of the vocabularies themselves.
5. Develop algorithms/tools for converting metadata based on the XML schema into RDF for the purposes of publication as Linked Data.

## Conference session outline

### Preparation (pre-conference)

User-stories, use-cases and other relevant position statements will have been solicited and gathered in this Github repository in advance of the session. At least one, and potentially several candidate solutions/recommendation will also have been outlined and added to this repository.

#### Purpose and scope

The main purpose of the session in Porto will be, therefore, to consider the candidate solutions in the context of the documented use-cases, and to attempt to reach a consensus on what should be recommended.

The workshop will constrain itself to the issue of how PIDs should be expressed in properties from the Dublin Core vocabularies, especially when serialised as XML/JSON. It will *not* attempt to develop a new metadata application profile for this domain. However, the application profiles already used in this domain may benefit immediately from a clear recommendation from DCMI on expressing PIDs.

#### Format

The session will probably be a half-day (approx. 4 hours). If the scope of this work grows - e.g. there are competing candidate solutions and string interest in these, then we may have to review this.

Attendance will be a mixture of invited people, with a call to go out to attract other interested parties nearer the time.

#### Intended output

The output will depend on the success of the discussions. If successful, the output of the workshop will be the basis of an official DCMI Recommendation or, possibly, revisions to the Dublin Core vocabularies themselves.
