---
title: "Per Resource Events"
abbrev: "prep"
category: std

docname: draft-gupta-httpbis-per-resource-events-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
area: "Applications and Real-Time"
workgroup: "HTTP"
keyword:
  - notifications
  - pubsub
venue:
  group: "HTTP"
  type: "Working Group"
  mail: "ietf-http-wg@w3.org"
  arch: "https://lists.w3.org/Archives/Public/ietf-http-wg/"
  github: "CxRes/id-pre-test-2"
  latest: "https://CxRes.github.io/id-pre-test-2/draft-gupta-httpbis-per-resource-events.html"

author:
 -
    fullname: Rahul Gupta
    email: cxres@protonmail.com

autolink-iref-cleanup: true
entity:
  protocol: Per Resource Events Protocol

normative:
  Delta: RFC3229
  HTTP: RFC9110
  HTTP-SF: I-D.ietf-httpbis-sfbis-03
  HTTP-Retrofit: I-D.ietf-httpbis-retrofit-06
  RFC822:
  RFC2046:
  RFC5789:
  RFC9112:
    -: HTTP1
    display: HTTP/1.1
  RFC9113:
    -: HTTP2
    display: HTTP/2
  SSE: W3C.eventsource

informative:
  FETCH:
    target: https://fetch.spec.whatwg.org
    title: Fetch - Living Standard
    date: false
  REST:
    target: https://roy.gbiv.com/pubs/dissertation/top.htm
    title: Architectural Styles and the Design of Network-based Software Architectures
    author:
      -
        ins: R.T. Fielding
        name: Roy T. Fielding
    date:
      month: September
      year: 2000
    refcontent: Doctoral Dissertation, University of California, Irvine
  RFC5322:
  RFC7838:
  RFC9205:
  WEBSUB: W3C.websub
  WS: W3C.websockets

--- abstract

Per Resource Events is a minimal protocol built on top of HTTP that allows clients to receive notifications directly from any resource of interest. The Per Resource Events Protocol (PREP) is predicated on the idea that the most intuitive source for notifications about changes made to a resource is the resource itself.

Minor change to draft for testing!

--- middle

<!-- Informative Sections -->

{::include src/sections/introduction.md}

{::include src/sections/design.md}

<!-- Conformance Section -->

{::include src/boilerplate/conformance.md}

{::include src/sections/conformance.md}

{::include src/sections/terminology.md}

<!-- Normative Sections -->

{::include src/sections/headers.md}

{::include src/sections/protocol.md}

{::include-nested src/sections/discovery.md}

{::include-nested src/sections/request.md}

{::include-nested src/sections/response-1.md}

{::include-nested src/sections/response-2.md}

{::include src/sections/rfc822.md}

--- back
