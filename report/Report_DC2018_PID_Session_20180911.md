## DC2018 session on "The Use Of Persistent Identifiers In Dublin Core Metadata"

Paul Walk, Tom Baker
2018-09-21

Scholarly publishers, repositories, and aggregators increasingly use persistent identifiers (PIDs) in their metadata to identify entities such as creators, publishers, subjects, and licenses.  A half-day session on September 11 at DC-2018 in Porto brought together stakeholders and metadata experts to consider alternative approaches for pairing literal values in Dublin Core-based metadata with relevant persistent identifiers (PIDs) -- for example, to identify a creator both by name and by ORCID or ISNI.  

Discussion in Porto focused on a [position paper](https://github.com/dcmi/pids_in_dc/blob/master/proposal/The_Association_of_Persistent_Identifiers_with_Literals_in_XML-formatted_Metadata_using_Dublin.md) that was prepared on the basis of a discussion of requirements on a [mailing list](https://groups.google.com/d/forum/pids-in-dublin-core) and [Github issue tracker](https://github.com/dcmi/pids_in_dc/issues).  The paper outlined two two alternative approaches: 

1. To use an XML attribute (`id=`) for adding a PID to an element holding a literal value:

```xml
<dc:creator id="https://orcid.org/0000-0003-1541-5631">Walk, Paul</dc:creator>
```

2. To use one or more DC Identifier elements in a nested description of the entity in
question:

```xml
<dc:creator>
	<dc:identifier>https://orcid.org/0000-0003-1541-5631</dc:identifier>
	<foaf:name>Walk, Paul</foaf:name>
</dc:creator>
```

Discussion in Porto weighed the useful simplicity of the former solution against the flexibility of the latter, which could in principle accommodate an arbitrary number of PIDs.  A strongly argued need to support multiple PIDs in practice appeared to tip the balance towards nested descriptions until it was pointed out that the value of an `id=` attribute could, in fact, allowably hold an arbitrary number of PIDs separated by whitespace or newlines:

```xml
<dc:creator id="https://orcid.org/0000-0003-1541-5631 http://paulwalk.net">Walk, Paul</dc:creator>
```

The simplicity of this approached tipped the balance back towards the use of an XML attribute.  This solution would not meet all requirements related to using PIDs in metadata, such as the need of some organizations to track the status and provenance of identity claims, but it was felt that such complex requirements were best met by specific application profiles.

This result will be described in draft DCMI Recommandation explaining how the proposed construct can be expressed with JSON, or with JSON-LD or RDF/XML for publication as Linked Data, and the draft specification will be posted for public comment.

