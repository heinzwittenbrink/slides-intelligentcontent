---
author: Heinz Wittenbrink
title: Intelligent Content und Content 4.0
institute: Master-Lehrgang Technische Dokumentation
date: 2017-10-13
---


# Intelligent Content - Content 4.0


# Zur Definition

---

> Intelligent content is content that is structured to optimize performance with technology. It is structurally rich, semantically categorized, automatically discoverable, reusable, reconfigurable, and adaptable. [@rockley2011]

---

> It means creating building blocks of content (content objects) that have been given meaning, by being tagged and structured so that computers can understand how to process those content objects. This allows content to be re-ordered, re-used, and otherwise manipulated so that you need less content to fulfill more needs, in an extremely agile way. [@bailie2015]


# Wozu intelligent content?

---

> It is only with intelligent content [] that it becomes possible to talk about a sustainable enterprise content strategy.[@rockley2011]

---

> An intelligent content strategy establishes a coherent plan under which content will be designed, developed and deployed so as to achieve maximum benefit to the customer and the organization while minimizing the cost to the organization. [@rockley2011]

---

## Automatisierung

> automation doesn't just happen. Content must be consciously designed to support it.[@rockley2011]

> If we design and prepare content in a way that is completely portable and open, then a wide range of applications can be used to automate common content tasks such as formatting.[@rockley2011]


# Wie sieht intelligent content aus?

---

> Intelligent content is content that is structurally rich and semantically categorized, and is therefore automatically discoverable, reusable, reconfigurable and adaptable.

---

![Figure 1. In many websites, the relationship between parts of content is implied in the presentation. But without that context, lacks an underlying structure.](https://spinsucks.com/wp-content/uploads/2017/01/photo1.png)

Bild: @hane2017

---

![Figure 2:The information is now structured into fields which store the content as data. This allows you to use it in any context.](https://spinsucks.com/wp-content/uploads/2017/01/photo2.png)

Bild: @hane2017

---


## Structurally rich

> Structure makes it possible to manipulate it.[@rockley2011]


## Semantically categorized

> Semantically categorized content [] is content that has been tagged with metadata to identify the kind of content within it.[@rockley2011]

## Easily discoverable


> Without semantic metadata it is very difficult to automatically, let alone manually, find the content we need.[@rockley2011]

​

> And when it is structurally rich, and assuming our content is in XML, we can use XQuery [], a standard that supports queries of XML data - not just XML files, but anything that can appear as XML, including databases.[@rockley2011]

---

> content mining[@rockley2011]



## Efficiently Resusable


> Reusable content [], content that is created once and used many times, reduces the time to create, manage and publish and reduces translation costs. We can create modular structured content that can either be easily retrieved for manual reuse or automatically retrieved for automated reuse.[@rockley2011]


## Dynamically Reconfigurable

​

> Knowing the structure of the content, we can output it to multiple channels reconfiguring it to best meet the needs of the channel, or we can automatically mix and match content to provide us with the information customers need []. We can even transform content (reconfigure it) from one structure to another,[@rockley2011]

## Completely Adaptable



> but content can be adapted (used in a different way), often without our knowledge, to meet a new need.[@rockley2011]


## Metadaten


> Unfortunately, applying metadata to a completed document means that it can only adequately describe the content at a very superficial level; it cannot identify the many types of content within the document.[@rockley2011]

## Standardisierung


# Was braucht man dazu in einer Organisation?

---

## Zentrale Content-Verantwortung

## Technischer Support

## Keine Silos


# Strategientwicklung

## Der Weg zum intelligent content: Content Strategie
> An intelligent content strategy establishes a coherent plan under which content will be designed, developed and deployed so as to achieve maximum benefit to the customer and the organization while minimizing the cost to the organization.[@rockley2011]

​--- 

> Technology. An effective strategy begins at the design stage, works through the authoring stage, ends at the delivery stage and is continually revisited to ensure it continues to meet the needs of authors, content and customers.[@rockley2011]

​

## Content Modellierung


> Content models. The information modeling process [] forces you to consider all information requirements (either for a specific project or within an entire organization) and to assess what information is available to fulfill those requirements. In an intelligent content strategy, the information model reflects the semantic structure of your information both at the information product level (for example, brochure) and at the element level (for example, value proposition).[@rockley2011]

---

![Content Model: Diagram](pics/lovinger_gibbon_models2.png){ width=70% }

Bild: @rachellovinger2013 


## Wiederverwendungsstrategie


​

> Reuse strategy. A reuse strategy identifies what types of content will be reused, the level of granularity, how the content will be reused and how to support authors in easily and effectively reusing it. Your strategy will depend upon your goals, your content, your authors and your selected technology.[@rockley2011]


## Taxonomy Strategy


> Taxonomy strategy. The taxonomy strategy enables you to intelligently store and retrieve your content based on a common vocabulary and shared metadata. In addition to traditional metadata for information storage and retrieval, it is important to develop metadata to define the delivery channel (print, web, wireless), the method of filtering the content (product, customer segment/audience, region, product version) and the final information product (brochure, web, eBook).[@rockley2011]

## Workflows


> Creating intelligent processes (workflow). An intelligent content strategy also involves people and intelligent (collaborative) processes. Collaboration ensures that the content elements are consistent and can be reused wherever they're required. Processes should be redesigned to match the intelligent content strategy and support the way the authors work. Workflow can be used to support these processes.[@rockley2011]


> We determined that the Darwin Information Typing Architecture (DITA) [] was appropriate for the content development. With DITA - an XML-based, end-to-end architecture for authoring, producing and delivering technical information - we could create structured, modular, reusable content [] that could be automatically adapted to each of the desired outputs (print, web, mobile). It also provided a strong support for translation.[@rockley2011]



# Implementierung


## XML

The role of XML. Everywhere you go, you hear about the use of XML. XML is being used on the web, in rich media and for content. While you don't have to use XML for your content, XML really helps make your content intelligent. Traditional office documents are simply files, and you have no access to the content because content is unstructured.[@rockley2011]

## XML und Content Delivery


> The power of XML for delivery. When it comes to delivering content, XML gives us a very wide range of options. In fact, part of the rationale for XML was to liberate content owners from being limited to providing only one or two delivery formats[@rockley2011]

---

## DITA: Maps

~~~ { .xml }
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE map
  PUBLIC "-//OASIS//DTD DITA Map//EN" "map.dtd">
<map>
  <title>The Project Gutenberg eBook of <ph
      outputclass="cite">The Mysterious Island</ph>, by Jules Verne</title>
  <topichead
    navtitle="License Statement">
    <topicref
      href="legalstuff/main-page.xml"/>
  </topichead>
  <topicref
    navtitle="The Mysterious Island"
    href="parts/title-page.xml"
    collection-type="sequence"/>
  <topicref
    href="parts/part-01.ditamap"
    format="ditamap"/>
  <topicref
    href="parts/part-02.ditamap"
    format="ditamap"/>
  <topicref
    href="parts/part-03.ditamap"
    format="ditamap"/>
  <topichead
    navtitle="end-of-book">
    <topicref
      href="legalstuff/end-of-book.xml"/>
  </topichead>
</map>
~~~

---


## XQuery

## DocBook

> DocBook does not support reuse as effectively as DITA, but it does provide a simpler conversion path from traditional business documents to XML.[@rockley2011]

## Component CMS


> Intelligent content needs an XML-aware system like a component content management system (CCMS) []. CCMS manage content at a granular (component) level of content, rather than at the page or document level.[@rockley2011]

# Ressourcen

## Events:

[Intelligent Content Conference](http://www.intelligentcontentconference.com/ "2017 Intelligent Content Conference Las Vegas, Nevada")

[Adobe DITA World 2017](https://2017-adobe-dita-world.meetus.adobeevents.com/ "Adobe DITA World 2017 - Adobe DITA World 2017 – The DITA Online Conference | Adobe Events")


## Literatur
