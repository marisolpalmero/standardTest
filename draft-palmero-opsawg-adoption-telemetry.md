---
title: "Yang data model specification for Adoption Telemetry"
abbrev: "Yang Spec for Adoption Telemetry "
docname: draft-palmero-opsawg-adoption-telemetry.md
category: info

ipr: trust200902
area: General
workgroup: OPSA Working Group
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: M. Palmero
    name: Marisol Palmero
    organization: Cisco Systems
    email: mpalmero@cisco.com

 -
    ins: J. Suhr
    name: Josh Palmero
    organization: Cisco Systems
    email: josuhr@cisco.com   

normative:
  

informative:



--- abstract

	This document proposes YANG modules for Adoption Telemetry.


--- middle

# Introduction

	Telemetry is the data automatically collected from deployed products to identify a product itself, how much it is being used, what are its top features, enabling the ability to turn on/off features, upgrading software, etc. This supports to primary use cases categories:
	* Product Adoption & Customer Value Proposition
	* Managed Service & Support

	Product vendors do not generate timely and consistent Telemetry data to mazimize customer experience

	This business specification focuses on MVP datasets and attributes for the needs of Adoption Telemetry: License & Product Inventory and Usage.
	Further Use Cases ranging from network automation and optimization to advanced and iterative issue remediation may require bidirectional connectivity and new datasets and attributes. These broader needs will be address on a following draft for Operations Telemetry.   


# Conventions and Definitions

	The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
	"SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this
	document are to be interpreted as described in BCP 14 {{RFC2119}} {{!RFC8174}}
	when, and only when, they appear in all capitals, as shown here.

	The following terms are defined in [RFC6241] and are used in this
	   specification:

	   o  configuration data

	   o  state data

	   The following terms are defined in [RFC7950] and are used in this
	   specification:

	   o  augment

	   o  data model

	   o  data node

	The terminology for describing YANG data models is found in [RFC7950].

1. Tree Diagrams

	   Tree diagrams used in this document follow the notation defined in
	   [RFC8340].

# Design of the Adoption Telemetry Data Model

	This model is used to obtain data inventory and usage from deployed products and solutions, it covers licenses, software components and inventory assets like devices, controllers, end-points, etc.
	 
	//EXPLAIN the modules ...

	The data model for Adoption Telemetry client has the following structure:

1. Tree Diagrams

2. Adoption Telemetry Client Modules


# Security Considerations

   The YANG module defined in this document is designed to be accessed
   via network management protocols such as NETCONF [RFC6241] or
   RESTCONF [RFC8040].  The lowest NETCONF layer is the secure transport
   layer, and the mandatory-to-implement secure transport is Secure
   Shell (SSH) [RFC6242].  The lowest RESTCONF layer is HTTPS, and the
   mandatory-to-implement secure transport is TLS [RFC8446].

   The NETCONF access control model [RFC8341] provides the means to
   restrict access for particular NETCONF or RESTCONF users to a
   preconfigured subset of all available NETCONF or RESTCONF protocol
   operations and content.


# IANA Considerations

1.  The IETF XML Registry

   This document registers TODO URIs in the IETF XML registry [RFC3688].
   Following the format in [RFC3688], the following registrations are
   requested:

      URI: urn:ietf:params:xml:ns:yang:ietf-adoption-telemetry-
      Registrant Contact: The OPSA WG of the IETF.
      XML: N/A, the requested URI is an XML namespace.



2.  The YANG Module Names Registry

   This document registers TODO XX YANG modules in the YANG Module Names
   registry [RFC7950].  Following the format in [RFC7950], the the
   following registrations are requested:


--- back

# Acknowledgments
{:numbered="false"}

	The authors wish to thank Jan Lindblad and many others for
   their helpful comments and suggestions.