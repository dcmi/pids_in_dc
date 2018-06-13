# PIDS in Dublin Core

## General description
DCMI has recently been approached  by several organisations dealing with metadata in the general domain of scholarly communications,  asking for clarification on how persistent identifiers should be included in Dublin Core metadata expressed in XML.

***Dublin Core metadata* is used here to mean metadata, typically formed in *records*, which use either the [DCMI Metadata Terms](http://www.dublincore.org/documents/dcmi-terms/) or the [Dublin Core Metadata Element Set](http://www.dublincore.org/documents/dces/)**. 

The domain of “scholarly communications” makes much use of the Dublin Core metadata in a number of application profiles (including one specified in the OpenAIRE Guidelines for repositories which have been adopted widely in Europe and South America). Within this domain there is currently a growing interest in the use of global persistent identifiers (PIDs) and a realisation that, without them, metadata is considerably less useful.
For a majority of cases in this domain, the most important resources to be identified with PIDs are:

* scholarly outputs (e.g publications, research data, software sources etc.) which are generally identified with either a DOI (in HTTP URI form) or with a general URL.
* authors and contributors - ORCID is becoming recognised as the conventional identifier agency for these, providing ORCID IDs (also in HTTP URI form)
* Organisations - especially funders, and also institutions with which authors are affiliated.

The exchange of metadata between systems in the scholarly communications economy is a key activity in that domain. Metadata is normally serialised and exchanged as either XML or JSON. The use of Dublin Core metadata is very common (with varying degrees of ‘precision’). The inclusion of PIDs in such metadata is somewhat arbitrary - many metadata records will contain one PID - identifying the subject of the record - but are less likely to contain any others, despite the record referencing identifiable resources (authors, organisations, other resources etc.)

## Workshop proposal
DCMI proposes a workshop, to be conducted in September at the [DCMI annual conference in Porto, Portugal](http://www.dublincore.org/conference/2018/), to consider how PIDs should be expressed in Dublin Core metadata records. 

The workshop will solicit use cases in advance, so that these may be considered on the day as ‘worked examples’. As an example (and one for which we know there is already interest), the workshop may consider the use-case of wishing to create a metadata record for a scholarly publication, which:

* uses Dublin Core properties such as dc:creator
* records multiple authors
* includes both string representations and PIDs for some of these authors, recognising that there may not be a PID for each of them
* includes some mechanism for ‘affiliating’ an author with an academic institution, using some other PID (ISNI perhaps) where available

There is also a particular interest in recommending best-practice for adoption in open-access repositories.

The workshop will constrain itself to the issue of how PIDs should be expressed in Dublin Core metadata, especially when serialised as XML/JSON. It will *not* attempt to develop a new metadata application profile for this domain. However several application profiles are already used in this domain, and especially in open-access repositories (e.g.  [OAI_DC](https://www.openarchives.org/OAI/openarchivesprotocol.html),  [OpenAIRE v4 (in beta)](http://openaire-guidelines-for-literature-repository-managers.readthedocs.io/en/latest/application_profile.html) and [RIOXX v2](http://www.rioxx.net/profiles/v2-0-final/)). These may benefit immediately from a clear recommendation from DCMI on expressing PIDs.

Attendance will be a mixture of invited people, with a call to go out to attract other interested parties nearer the time. We will use the time between now and the conference to solicit some uses cases and begin the discussion in advance of the workshop.

The output will depend on the success of the discussions. If successful, the output of the workshop will be the basis of an official DCMI Recommendation.
