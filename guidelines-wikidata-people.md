# Guidelines for Using Wikidata to Mobilize Information about People in Collections: A Paleontology Perspective

[insert cool image to jazz up this front page]

_Created by:_ (authors listed alphabetically) [Jennifer Bauer](https://orcid.org/0000-0002-6337-6270), [Roger Burkhalter](https://orcid.org/0000-0001-5518-5661), [Talia Karim](https://orcid.org/0000-0001-6514-963X), [Erica Krimmel](https://orcid.org/0000-0003-3192-0080), Margaret Landis, [Siobhan Leachman](https://orcid.org/0000-0002-5398-7721), [Holly Little](https://orcid.org/0000-0001-7909-4166), [Malena Lorente](https://orcid.org/0000-0002-3723-0710), [Suzanne K. Mills](https://orcid.org/0000-0002-3759-694X), Nicole Neu-Yagle, [Ben Norton](https://orcid.org/0000-0002-5819-9134), [Deborah Paul](https://orcid.org/0000-0003-2639-7520), [David Shorthouse](https://orcid.org/0000-0001-7618-5230), [Jessica Utrup](https://orcid.org/0000-0001-5201-8235), [Jacob Van Veldhuizen](https://orcid.org/0000-0001-6770-0181), [Lindsay Walker](https://orcid.org/0000-0002-2162-6593), and with input from participants of the "Using Wikidata to Capture and Share Information about People in Paleontology" workshop (March 2022).

_Publishing date_: 2022-XX-XX

_License_: [CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)

_Should you wish to credit this document, please cite as:_[add once we have determined where to share]

_This document was inspired by and draws content from:_ Siobhan Leachman. 2020. Wikidata Notes for Bat Collectors. [https://doi.org/10.5281/zenodo.4724139](https://doi.org/10.5281/zenodo.4724139).

**Table of Contents**

[Introduction](#_9ys7z8mwju2o)

[Purpose of this document](#_7yz53g7hrnt5)

[Why use Wikidata?](#_uwyf8ndswl2z)

[Best practices for mobilizing information about people](#_ja25pmnh2rej)

[Respect Privacy](#_ktcyr6oalqml)

[Maintain Objectivity](#_o2m962f833ps)

[Glossary](#_im5ca43d34jm)

[Contributing to Wikidata](#_xcc8unbufbi6)

[Create a new account and log in](#_i3l6qnytp4i)

[Search for an existing item](#_uptflaizl9s3)

[Quick search using the search box](#_6hyfe3y9askm)

[Comprehensive search using the Query Service](#_filf3fedmym3)

[Create a new item](#_yknsxhra26cx)

[Add statements](#_2z7vn8bqd6sz)

[Wikidata items to use as exemplars](#_gjlulwkzfci3)

[Add references](#_76qxzuercrnh)

[Tools for references](#_elq44hq45qs)

[Selecting high quality references](#_1ipnlhma0t3g)

[Archiving unstable URLs](#_yjf6ogqhq5z3)

[Analog references](#_6gyc2z7vh8au)

[Add external identifiers](#_mgp05lfms8bs)

[Merge items](#_9v584so5cyv2)

[Edit in bulk](#_b9wiv83cy9bc)

[QuickStatements](#_a1xc29j9mk0i)

[OpenRefine Wikidata Plugin](#_96rwifea2wn5)

[Scripting](#_8tj03l5izadg)

[Querying Wikidata](#_93iyd0nkxbo)

[Wikidata Query Builder](#_4oz9mla8n9ht)

[SPARQL](#_3xfks9vwxkhz)

[Using Wikidata outside of Wikidata](#_phm41tosmox1)

[Exporting From Wikidata in Bulk](#_mszb3fdw5lqp)

[Export with Wikidata Query Service](#_ey5n81sngvqm)

[Export with MediaWiki Action API](#_bm7v635dj6fk)

[Export with REST API](#_6fhi6ekvnl8g)

[Export with JSON Data Dump](#_c7rkr9w3n9ss)

[Export with RDF Data Dump](#_eij0or5x6m5f)

[Wikidata Toolkit](#_hesroemw5b34)

[Resources](#_kkx34hsvjvdp)

[Resources for discovering biographical information](#_skvnrilfzq5k)

[Resources for using Wikidata](#_lve879ltui7f)

[Resources for exploring Wikidata](#_5kk40cklds7j)

[Resources for getting involved in the Wikimedia community](#_titv9dqwe27l)

[Conclusion](#_yv0q8m6257kg)

[Appendix A. Recommended Wikidata Properties](#_92clws2v26zl)

[Appendix B. External Identifiers for People](#_4fhqfmhbj91v)

##


## Introduction

## Purpose of this document

The purpose of this document is to provide a framework for how to mobilize information via Wikidata about people working in and/or associated with scientific collections. Building on previous Wikidata documentation produced by Siobhan Leachman (2020, [https://doi.org/10.5281/zenodo.4724139](https://doi.org/10.5281/zenodo.4724139)), participants of the _Using Wikidata to Capture and Share Information about People in Paleontology_ workshop (held March 29-31, 2022) created this framework to formalize and share practical knowledge gained from the workshop.

## Why use Wikidata?

Collections professionals often focus on sharing information about specimens by publishing via online data aggregators such as the Global Biodiversity Information Facility (GBIF, [https://www.gbif.org/](https://www.gbif.org/)) or the iDigBio Portal ([https://www.idigbio.org/portal/](https://www.idigbio.org/portal/)). The focus of the majority of collections information work has been, primarily, on mobilizing the what, where, and when of a specimen and less on the people involved in collection and preparation. However, knowing definitively who was involved with a specimen—by collecting, identifying, preparing, georeferencing, conducting research on, etc.—enhances the ways in which specimen data can be used. For example, information about birth, death, and occupation dates may help constrain specimen collection dates where they are not explicitly known.

Currently, biographical information and the curatorial effort to maintain this information tend to be duplicated across scientific collection databases and institutions. Wikidata offers a centralized, independent platform for working collaboratively to disambiguate people associated with collections and to mobilize biographical information about them. For example, aliases and other biographical information captured in Wikidata by collections staff with deep knowledge about a person can help staff at another collection disambiguate an obscure namestring associated with some of their specimens. Once a person is represented in Wikidata, they are associated with a unique Wikidata identifier (i.e., a [Wikidata QID](https://www.wikidata.org/wiki/Q43649390)). Wikidata identifiers underpin the ability to transfer information about people programmatically, thereby facilitating data completeness, accuracy, and redundancy between local collection databases, Wikidata, and various other online databases and collections management systems.

Storing biographical information in Wikidata makes it more discoverable as part of the Linked Open Data ecosphere. For example, queries on Google's search engine return results from Wikidata (Figure 1). As a centralized repository of linked data, Wikidata also provides ways to demonstrate who is doing what work across multiple collections, and with what impact. This has potential to increase inclusion and improve equity, as many people associated with scientific collections have yet to be fully acknowledged for their contributions, especially historical people who were female, non-White, Indigenous, and/or of lower social or educational standing. The process of creating, editing, and linking information in Wikidata is inherently transparent and encourages removing silos and sharing expertise.

![](RackMultipart20220809-1-5enz3r_html_9c3395a61ec947fa.png)

Figure 1. Screenshot from Google ([https://www.google.com](https://www.google.com/), retrieved 2022-04-25) illustrating how its search engine presents structured data via the "Knowledge Panel" in the right hand sidebar. These data come from the Google Knowledge Graph, which in turn draws from various sources including Wikidata.

## Best practices for mobilizing information about people

Wikidata provides public access to extensive information about many topics. When those topics are people, being sensitive to how data about them is publicly shared is not only good manners, it also helps maintain Wikidata as an accurate data repository that is safe and respectful for all users. The following considerations should be taken into account when entering data.

### Respect privacy

When creating or editing a Wikidata item for a living person, there are privacy issues to consider (see the [Wikidata policy on Living People](https://www.wikidata.org/wiki/Wikidata:Living_people)). Remember that the data being provided about a subject is publicly available and can include personal information such as, but not limited to: name, age, sex, gender, marital status, spouse's name, and nationality. The subject of the item may not want to have this level of personal information about them visible to a broad audience and may even want the item taken down. If that living person is you, creating an autobiographical item is not recommended as it may be flagged by Wikidata for removal. Instead, ask a colleague to create a Wikidata item for you!

Out of concerns for safety and possible legal ramifications, Wikidata items for living minors (e.g., individuals 18 years of age or younger in the United States) should not be created.

### Maintain objectivity

Data entered into Wikidata should be factual rather than based on opinion. To maintain an objective rather than subjective perspective, it is considered best practice not to make a Wikidata item for yourself, as described above.

## Glossary

A glossary of commonly used Wikidata terms can be found here: [https://www.wikidata.org/wiki/Wikidata:Glossary](https://www.wikidata.org/wiki/Wikidata:Glossary)

## Contributing to Wikidata

The best way to get acquainted with how Wikidata works is to contribute to it yourself. You do not need to be an expert, and the learning curve is gentle. The steps below will guide you through creating and editing a new Wikidata item, using examples most directly relevant to people associated with paleontology collections.

For a visual orientation to contributing, please see this 20-minute long recording originally presented by Jessica Utrup at the _Using Wikidata to Capture and Share Information about People in Paleontology_ workshop: [https://vimeo.com/702109576](https://vimeo.com/702109576).

## Create a new account and log in

To create and edit Wikidata items, you need to have a Wikimedia account. This account is connected to all Wikimedia projects, including Wikipedia and Wikidata. If you already have an account, skip to step 4 below.

1. To create a new account, start at the main Wikidata page here: [https://www.wikidata.org/wiki/Wikidata:Main\_Page](https://www.wikidata.org/wiki/Wikidata:Main_Page)
2. Click _Create Account_ at the top right of this page (Figure 2). Fill out the form and click the blue _Create your account_ button. Record your username and password so that you can log in again at a later date.

![](RackMultipart20220809-1-5enz3r_html_407e9ca794fb2e09.png)

Figure 2. Screenshot from Wikidata ([https://www.wikidata.org](https://www.wikidata.org/), retrieved 2022-05-05) indicating where to create an account and/or log in.

1. When creating a new account, it is helpful to other users to include some information about yourself on your personal user page. This lets the community know who you are and what you are interested in working on in Wikidata. For example, see the user page for Wikidata superuser Siobhan Leachman here: [https://www.wikidata.org/wiki/User:Ambrosia10](https://www.wikidata.org/wiki/User:Ambrosia10). Siobhan's page includes information about herself and the projects she has worked on, including notes that serve as useful memory aids for her and others.

1. If you already have an account, use your username and password to log in on the main Wikidata page here: [https://www.wikidata.org/wiki/Wikidata:Main\_Page](https://www.wikidata.org/wiki/Wikidata:Main_Page).

## Search for an existing item

Once logged in, you can create new items and edit existing ones. To prevent duplicating an existing item, it is critical to first search for the item in Wikidata. The two primary ways to search for an existing item are described below.

### Quick search using the search box

One option is to do a quick search for an existing item (e.g., a person) using the Wikidata search box at the upper right of your screen (Figure 3).

![](RackMultipart20220809-1-5enz3r_html_4a934447d4736114.png)

Figure 3. Screenshot from Wikidata ([https://www.wikidata.org](https://www.wikidata.org/), retrieved 2022-05-05) indicating where the quick search box is located.

The search box is a quick way to locate an item already in Wikidata, but the results will be broad. For example, if you type "paleontologist" into the search box, the results will return not only the profession of "paleontologist" ([https://www.wikidata.org/wiki/Q1662561](https://www.wikidata.org/wiki/Q1662561)), but also people that have "paleontologist" in their description, locations with "paleontologist" in their name, and journal articles or books that have "paleontologist" as part of the title. The search box is also sensitive to spelling variations, e.g., "palaeontologist" will produce different results than "paleontologist." To help refine your search results, use the Wikidata Query Service as described below.

### Comprehensive search using the Query Service

A second option is to use Wikidata's Query Service, which helps refine search results based on specific criteria. Using this will make it easier for you to find what you are looking for, or else to confirm that what you are looking for does not yet exist in Wikidata. To access, select _Query Service_ from the sidebar on the left side of the main page, or else access it directly from this link: [https://query.wikidata.org/](https://query.wikidata.org/).

You can search with the Query Service by either: (1) using the more visual Wikidata Query Builder, or (2) writing a query using the SPARQL language. To learn more about these options, see the detailed instructions provided below in the section [Querying Wikidata](#_93iyd0nkxbo).

## Create a new item

Before creating a new item, be sure you have searched carefully to ensure that the item—in this case, a person—is not already in Wikidata (see previous section). If you are uncertain that an existing Wikidata item represents the person you are adding information for, it is appropriate to create a new item and potentially merge the two items later if they are confirmed to represent the same person (see [Merge items](#_9v584so5cyv2), below).

As a reminder, you must be logged into Wikidata to create a new item.

1. Select _Create a new item_ from the sidebar on the left side of any Wikidata page.
2. You will be directed to an editing interface (Figure 4) to enter data for the following fields:
  1. The _Language_ field refers to the language you are using to edit this Wikidata item.
  2. The _Label_ field is the name by which the person is most well known, e.g., the name under which the person published. For example, "[Charles Schuchert](https://www.wikidata.org/wiki/Q2623977)" or "[Julia Anna Gardner](https://www.wikidata.org/wiki/Q15999449)."
  3. The _Description_ field provides space for a tagline about who this person is and/or what they do. This description is displayed underneath the _Label_ value and can be a useful way of quickly disambiguating different people in Wikidata search results (Figure 5). The preferred format for a description includes country of citizenship and occupation(s) followed by birth and death years, e.g., "American paleontologist (1858 –1942)." Refer to the country of citizenship following the same language norms that Wikidata uses elsewhere, e.g., "[Americans](https://www.wikidata.org/wiki/Q846570)" for people from the United States of America.
  4. The _Aliases_ (or _Also known as_) field is highly important for disambiguation. All variations of a person's name should be included in this field, using a pipe character ("|") to separate each variation, e.g., "C. Schuchert | C Schuchert | Chas Schuchert." Alternatively, aliases can also be added after creating the new item. Aliases help humans and computers (including Wikidata bots) link items to external identifiers, and they also help others find this item more easily when using the Wikidata search box.

![](RackMultipart20220809-1-5enz3r_html_382b6b4ee39bcd6f.png)

Figure 4. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Special:NewItem](https://www.wikidata.org/wiki/Special:NewItem), retrieved 2022-05-05) showing the form to create a new item.

1. Press the blue _Create_ button at the bottom left of the form to publish the new item to Wikidata. You will be redirected to a new page displaying the information you just entered (Figure 5).

![](RackMultipart20220809-1-5enz3r_html_1824c5844eb9f65e.png)

Figure 5. Screenshot of Charles Schuchert's Wikidata item ([https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977), retrieved 2022-05-05) showing his description and aliases.

1. Don't stop here! To avoid having Wikidata's tidying bots remove your newly created item, you need to flesh it out by adding statements about this person. Proceed to the next section for further instructions on adding statements.

## Add statements

Wikidata statements capture data about the item. For an item representing a person, you may have statements for data such as their place and date of birth, education level, or employer. [Statements](https://www.wikidata.org/wiki/Help:Statements) start with a [property](https://www.wikidata.org/wiki/Help:Properties) which is then linked to a value, which can be circumscribed by a [qualifier](https://www.wikidata.org/wiki/Help:Qualifiers) and should almost always be supported by a [reference](https://www.wikidata.org/wiki/Help:Sources) (Figure 6). Depending on the property, most values will also be a Wikidata item, but some will be unlinked text strings. For example, the property of "[country of citizenship (P27)](https://www.wikidata.org/wiki/Property:P27)" could be linked to the value of "[United States of America (Q30)](https://www.wikidata.org/wiki/Q30)" (where this value is another Wikidata item), and the property of "[pseudonym (P742)](https://www.wikidata.org/wiki/Property:P742)" could be linked to the value of "Jane Doe" (where this value is a text string). Wikidata will prompt you to conform your value to the data type and format that each property expects.

![](RackMultipart20220809-1-5enz3r_html_d86831201d732175.png) ![](RackMultipart20220809-1-5enz3r_html_455f72bdd714b858.png)

Figure 6. Screenshots from Wikidata ([https://www.wikidata.org/wiki/Q15999449](https://www.wikidata.org/wiki/Q15999449), retrieved 2022-05-11) indicating how properties, values, qualifiers, and references are related in the interface for viewing (left) and editing (right) statements.

There are thousands of properties that can be included as statements on a Wikidata item (see [https://www.wikidata.org/wiki/Wikidata:List\_of\_properties](https://www.wikidata.org/wiki/Wikidata:List_of_properties)). To narrow this down, [Appendix A](#_92clws2v26zl) lists recommended properties to add to the item of a person who is associated with scientific collections. The list of properties in Appendix A is just a starting place and is not exhaustive. The rows in Appendix A marked with an asterisk (\*) are properties that provide personal information and should be used with caution when creating or editing an item for a living person.

The first statement you need to make is one that will tell Wikidata your item represents a person.

1. Click the _+ add statement_ button on the item, causing a new statement box to appear (Figure 7).
2. In the left (_Property_) text box, enter the property "[instance of (P31)](https://www.wikidata.org/wiki/Property:P31)."
3. In the right text box, enter the value "[human (Q5)](https://www.wikidata.org/wiki/Q5)."
4. Click the _publish_ button in the top right of the statement box (Figure 7). This will save your statement to the Wikidata item.

![](RackMultipart20220809-1-5enz3r_html_60f4d1146384acd0.png)

Figure 7. Screenshot from Wikidata ([https://www.wikidata.org](https://www.wikidata.org/), retrieved 2022-05-11) illustrating where the _+ add statement_ button and _publish_ buttons are located.

### Add qualifiers

Now that Wikidata knows your item represents a human, it will suggest other properties to include that relate to people. You can add additional information in the form of qualifiers to these properties. To do this, you will:

1. Click the _+ add statement_ button on the item, causing a new statement box to appear.
2. In the left text box, enter the property you wish to use, e.g., "[employer (P108)](https://www.wikidata.org/wiki/Property:P108)."
3. In the right text box, enter the value to be linked with that property, e.g., "[Natural History Museum of Los Angeles County (Q2502709)](https://www.wikidata.org/wiki/Q2502709)." You will encounter instances where the value you want to link is not accepted by Wikidata, and an error message of "No match was found" is displayed below the text box. This occurs because the property you are making a statement about requires the value to be a Wikidata item and your value does not already exist in Wikidata as an item. In this case, open a new browser tab and create a Wikidata item for the value that you want to link. Once created, return to the person's item and retype the value in the statement.
4. If appropriate, add one or more qualifiers to the value by clicking the _+ add qualifier_ button. Qualifiers are like statements within a statement, and as such consist of a property-value pair. For example, you could enter qualifiers to record the tenure of a person's employment at an institution, e.g., "[start time (P580)](https://www.wikidata.org/wiki/Property:P580)" = "1940" and "[end time (P582)](https://www.wikidata.org/wiki/Property:P582)" = "1972."
5. Add a reference by clicking the _+ add reference_ button. See the next section, [References](#_76qxzuercrnh), for more detailed information.
6. Click the _publish_ button in the top right of the statement box. This will save your statement to the Wikidata item. If you included qualifiers in your statement and Wikidata shows a warning exclamation point in a circle, this means that the qualifier you used is not valid for this property. Go back and edit the statement to replace the invalid qualifier with a valid one.
7. If appropriate, add another value to be linked with the same property. For example, a person may have been employed by multiple institutions throughout their career and you will want to record that information. Each institution can be linked to the employer property statement for a more complete record of the person's employment history. To add additional values to a property, click the _+ add value_ button (Figure 8), include a reference and qualifier(s) if appropriate, and save by clicking the _publish_ button.

![](RackMultipart20220809-1-5enz3r_html_5c572ed66effd98c.png)

Figure 8. Screenshot from Wikidata ([https://www.wikidata.org](https://www.wikidata.org/), retrieved 2022-05-11) illustrating where the _+ add value_ button is located.

1. Click the _publish_ button in the top right of the statement box. This will save your statement to the Wikidata item.

Note: Statements can only be linked to one property, but properties can have more than one linked value.

### Wikidata items to use as exemplars

The following people have robust Wikidata items with many statements and are relevant to the domain of paleontology. You may find it helpful to browse their Wikidata items for ideas on what statements might fit your new item, and for illustrations of how to use different properties.

- Charles Schuchert, [https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977)
- Winifred Goldring, [https://www.wikidata.org/wiki/Q8025390](https://www.wikidata.org/wiki/Q8025390)
- Julia Anna Gardener, [https://www.wikidata.org/wiki/Q15999449](https://www.wikidata.org/wiki/Q15999449)
- Wilmatte Porter Cockerell, [https://www.wikidata.org/wiki/Q19865330](https://www.wikidata.org/wiki/Q19865330)
- Theodore Dru Alison Cockerell, [https://www.wikidata.org/wiki/Q2506718](https://www.wikidata.org/wiki/Q2506718)
- Alfred Romer, [https://www.wikidata.org/wiki/Q688766](https://www.wikidata.org/wiki/Q688766)

## Add references

Statements made in Wikidata should be verifiable facts supported by references. [References](https://www.wikidata.org/wiki/Help:Sources), also called sources, provide other Wikidata users with a way to check your information, and they are especially important when a single property has multiple, conflicting values. The only types of statements that regularly do _not_ require a reference are ones that document common knowledge, e.g., "[instance of (P31)](https://www.wikidata.org/wiki/Property:P31)" + "[human (Q5)](https://www.wikidata.org/wiki/Q5)."

1. Add a reference to a statement that you are editing by clicking the _+ add reference_ button in the statement editing box (Figure 9).

![](RackMultipart20220809-1-5enz3r_html_871ce382c6431b78.png)

Figure 9. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Q15999449](https://www.wikidata.org/wiki/Q15999449), retrieved 2022-05-11) illustrating where the _+ add reference_ and _+ add_ buttons are located.

1. Enter the reference property in the first box. Typically the property used for references is either "[stated in (P248)](https://www.wikidata.org/wiki/Property:P248)" (for publications or media, Figure 10) or "[reference URL (P854)](https://www.wikidata.org/wiki/Property:P854)" (for websites or online sources, Figure 11). "[DOI (P356)](https://www.wikidata.org/wiki/Property:P356)" can also be used.

![](RackMultipart20220809-1-5enz3r_html_4c989cd53b87a6a9.png)

Figure 10. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977), retrieved 2022-05-05) showing Charles Schuchert's position held as the president of GSA with a "stated in" reference.

![](RackMultipart20220809-1-5enz3r_html_18ce88437bb2a584.png)

Figure 11. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977), retrieved 2022-05-05) showing that Charles Schuchert's archives are held at Yale, as supported by a "reference URL" reference.

1. After you have entered a reference property, a second box will appear for you to enter the reference value. Note that whereas "[reference URL (P854)](https://www.wikidata.org/wiki/Property:P854)" expects a text string, "[stated in (P248)](https://www.wikidata.org/wiki/Property:P248)" expects your value to be another Wikidata item. In this case, open a new browser tab and create a Wikidata item for the value that you want to link. Once created, return to the person's item and retype the reference value in the statement.
2. If you entered a value for "[reference URL (P854)](https://www.wikidata.org/wiki/Property:P854)," then you should also include a second property for "[retrieved (P813)](https://www.wikidata.org/wiki/Property:P813)," using the date you accessed the reference URL as your value. Add this by clicking the _+ add_ button in the blue reference statement editing box (Figure 9).
3. Click the _publish_ button in the top right of the statement box. This will save your new reference statement to the Wikidata item.

### Tools for references

Wikidata has several tools that make adding the same reference to multiple statements significantly easier than it would be to do so manually. The most useful tool is called _DuplicateReferences_, and you can add it to your user account by following these instructions:

1. Near your username on the upper right side of any Wikidata page, select _Preferences_ (Figure 12).

![](RackMultipart20220809-1-5enz3r_html_40d1dc7efd7d1937.jpg)

Figure 12. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Special:Preferences](https://www.wikidata.org/wiki/Special:Preferences), retrieved 2022-05-05) showing the navigation links for _Preferences_ and _Gadgets_.

1. From the tabs on your _Preferences_ page, select _Gadgets_ (Figure 12).
2. Scroll down through the list of gadgets and check the box next to _DuplicateReferences_ (see Figure 13).

![](RackMultipart20220809-1-5enz3r_html_4e2de69bda3428ab.png)

Figure 13. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Special:Preferences](https://www.wikidata.org/wiki/Special:Preferences), retrieved 2022-05-05) showing the selection that needs to be made to allow you to copy references.

1. Check that this gadget has been successfully added to your account by returning to a Wikidata item that you would like to add references to.
2. To use the _DuplicateReferences_ gadget, expand the _References_ dropdown on any statement and look for a _copy_ button on the right hand side (Figure 14). Click _copy_ and navigate to another statement for which you want to add the same reference. Expand the _References_ dropdown on this statement editing box, and click on _insert reference_ on the bottom right. You should see the reference statement appear, and it is published automatically.

![](RackMultipart20220809-1-5enz3r_html_1295813ecddf3982.png)

Figure 14. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977), retrieved 2022-05-05) showing the _copy_ reference link that is now visible.

### Selecting high quality references

References vary in quality. A detailed overview of references in Wikidata can be found in _Amaral G., et al. 2021. Assessing the quality of sources in Wikidata across languages: A hybrid approach. Journal of Data and Information Quality 13(4): 1-35._ [_https://doi.org/10.1145/3484828_](https://doi.org/10.1145/3484828).

A [list of resources](#_skvnrilfzq5k) where you will find biographical information is provided in this document, but generally looking for memorials and obituaries in journals published by professional societies (e.g., _Journal of Paleontology_ published by The Paleontological Society) is a good place to start.

### Archiving unstable URLs

If you would like to use a website as a reference via the "[reference URL (P854)](https://www.wikidata.org/wiki/Property:P854)" property, but are concerned that it may disappear, consider adding the URL to the [Internet Archive Wayback Machine](https://archive.org/web/). You can then use the URL provided by Internet Archive. For more information about the Wayback Machine, what it does, and how to save URLs to the Wayback Machine, see [this video](https://www.youtube.com/watch?v=ts1tu1BiSuY&ab_channel=InternetArchive).

### Analog references

In some cases you might need to cite an analog reference (e.g., a field trip guide or the newsletter of a local paleontological club). If the document could be digitized, and is out of copyright or openly licensed, you may consider uploading it to the Internet Archive. See an example tutorial of how to upload to Internet Archive in [this PDF](https://moorefreelibrary.org/wp-content/uploads/2020/11/Workshop-2-2-Uploading-Media-to-the-Internet-Archive.pdf).

Where uploading the analog reference to Internet Archive is not feasible, you will need to create or find an item in Wikidata to represent the analog reference (Figure 15). Many analog references already exist as Wikidata items, so just as when creating a new item for an individual in Wikidata, first search for an analog reference before adding it as a new item.

![](RackMultipart20220809-1-5enz3r_html_84a0c27059b5d95b.jpg)

Figure 15. Screenshots from Wikidata ([https://www.wikidata.org/wiki/Q111968550](https://www.wikidata.org/wiki/Q111968550) and [https://www.wikidata.org/wiki/Q111968914](https://www.wikidata.org/wiki/Q111968914), retrieved 2022-05-11) illustrating an option for referencing an analog source (a printed newsletter named "Bryozoa") by creating a new Wikidata item for it.

## Add external identifiers

External identifiers link information compiled by a recognized authority about an individual to the individual's Wikidata item. Adding these identifiers is a very important part of creating Wikidata items that are integrated into the Linked Open Data world. External identifiers are a special type of statement, and adding them is essentially the same process as described above in [Add statements](#_2z7vn8bqd6sz). You can add an external identifier by following these steps:

1. Click the _+ add statement_ button on the item, causing a new statement box to appear.
2. In the left text box, search for the property that represents the external identifier, e.g., "[VIAF ID (P214)](https://www.wikidata.org/wiki/Property:P214)." The most important external identifiers to add are: [VIAF ID (P214)](https://www.wikidata.org/wiki/Property:P214), [ISNI (P213)](https://www.wikidata.org/wiki/Property:P213), [ORCID iD (P496)](https://www.wikidata.org/wiki/Property:P496), and [WorldCat Identities ID (P7859)](https://www.wikidata.org/wiki/Property:P7859). See [Appendix B](#_4fhqfmhbj91v) for a more complete list of external identifiers relevant to people, and where to look for them.
3. In the right text box, enter the value for the identifier.
4. You do not need to provide a reference for an external identifier. However, adding a reference statement that includes the "[retrieved (P813)](https://www.wikidata.org/wiki/Property:P813)" property provides a data point should any changes happen to the external identifier in the future.
5. Click the _publish_ button in the top right of the statement box. This will save your statement to the Wikidata item.

Wikidata separates identifier statements into a section called _Identifiers_. You won't see this section on your item until you add an external identifier statement, at which point Wikidata will automatically create it (Figure 16).

![](RackMultipart20220809-1-5enz3r_html_2487417c84d0059.png)

Figure 16. Screenshot from Wikidata ([https://www.wikidata.org/wiki/Q2623977](https://www.wikidata.org/wiki/Q2623977), retrieved 2022-05-11) showing the top of the _Identifiers_ section on Charles Schuchert's item.

## Merge items

Despite the best efforts of its users, Wikidata does contain duplicate items (e.g., two Wikidata items representing the same person). Duplicate items should be merged so that all information about a person can be found within a single Wikidata item. More information about how to merge duplicate items can be found here: [https://www.wikidata.org/wiki/Help:Merge](https://www.wikidata.org/wiki/Help:Merge).

## Edit in bulk

Bulk editing in Wikidata can be ideal for situations where you already have complex and potentially a lot of data, and you are uncertain what, if any, of that data is already represented in Wikidata. There are several primary options for editing Wikidata in bulk: QuickStatements, OpenRefine, and scripting. Each of these is outlined below. Prior to using any of these bulk editing options, you should familiarize yourself with the way Wikidata organizes information by editing directly in the Wikidata user interface. This will help you understand how and when to use the bulk editing tools effectively.

For a visual orientation to bulk editing in Wikidata, including a live demo focused on OpenRefine, please see this hour-long recording originally presented by Erica Krimmel at the _Using Wikidata to Capture and Share Information about People in Paleontology_ workshop: [https://vimeo.com/702109441](https://vimeo.com/702109441).

In addition to the bulk editing options described here, Wikidata bots are also actively editing content via automated workflows. You can learn more about Wikidata bots at [https://www.wikidata.org/wiki/Wikidata:Bots](https://www.wikidata.org/wiki/Wikidata:Bots).

### QuickStatements

QuickStatements is a commonly used tool to create new statements in Wikidata by uploading a spreadsheet. QuickStatements reviews uploaded edits for duplicate statements and maintains audit tracking for every edit action.

- Access QuickStatements: [https://www.wikidata.org/wiki/Help:QuickStatements](https://www.wikidata.org/wiki/Help:QuickStatements)

### OpenRefine Wikidata Plugin

The major benefit of using OpenRefine to make bulk edits in Wikidata is that you can work entirely in one visual interface to discover existing data, edit or create new data, and upload new data to Wikidata. While working with data in OpenRefine, Wikidata can be accessed as a reconciliation service to validate information. OpenRefine version 3.0 or later includes integrated support for this use of Wikidata.

- See documentation from Wikidata: [https://www.wikidata.org/wiki/Wikidata:Tools/OpenRefine](https://www.wikidata.org/wiki/Wikidata:Tools/OpenRefine)
- See documentation from OpenRefine: [https://docs.openrefine.org/manual/wikibase/reconciling](https://docs.openrefine.org/manual/wikibase/reconciling)
- See this OpenRefine tutorial from WikidataCon 2021: ​​[https://www.youtube.com/watch?v=5HlPol\_-n3o](https://www.youtube.com/watch?v=5HlPol_-n3o)

### Scripting

Wikidata allows access via bots for scripts written in programming languages such as Python. These scripts commonly use QuickStatements as an intermediary tool.

- See PyWikiBot: [https://pypi.org/project/pywikibot/](https://pypi.org/project/pywikibot/)
- See Wikidataintegrator: [https://github.com/SuLab/WikidataIntegrator](https://github.com/SuLab/WikidataIntegrator)

## Querying Wikidata

As discussed above, the search box interface in Wikidata can limit your results, and you may therefore wish to use more comprehensive methods for querying. Here, we describe methods for using the Wikidata Query Builder and SPARQL. Additional information and tutorials on how to query Wikidata can be found here:

[https://www.wikidata.org/wiki/Wikidata:SPARQL\_query\_service/Wikidata\_Query\_Help](https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/Wikidata_Query_Help)

### Wikidata Query Builder

Wikidata's Query Builder service is designed to be easy to use for those with minimal programming experience. You can even build a query without knowing all of the property and item numbers (Figure 17).

![](RackMultipart20220809-1-5enz3r_html_eace5470e654aec3.png)

Figure 17. Screenshot from Wikidata Query Builder ([https://query.wikidata.org/querybuilder/](https://query.wikidata.org/querybuilder/), retrieved 2022-05-11) illustrating the user-friendly interface and highlighting key elements.

Follow the steps below for an example of how you might use the Wikidata Query Builder:

1. Go to the Wikidata Query Builder interface at [https://query.wikidata.org/querybuilder/](https://query.wikidata.org/querybuilder/).
2. Start typing "occupation" into the _Property_ field (Figure 17). A list of options will auto-populate, and you can select the correct property by clicking on it.
3. Start typing "paleontologist" in the _Value_ field (Figure 17). A list of options will auto-populate, and you can select the correct value by clicking on it.
4. To see more than 100 items, uncheck the box _Limit the number of results to_ or change the number in the box (Figure 17).
5. Click the _Run query_ button to execute the query (Figure 17). The results will appear in a table under the _Results_ header.
6. To further manipulate this data, hover over the table and download the results in a variety of formats including JSON, TSV, CSV, HTML, SVG (Figure 18).

![](RackMultipart20220809-1-5enz3r_html_4968a5479e0bba62.png)

Figure 18. Screenshot from Wikidata Query Builder ([https://w.wiki/59cd](https://w.wiki/59cd), retrieved 2022-05-11) showing the results of the example query above and highlighting how to download these data.

### SPARQL

Creating a new query using SPARQL requires some programming knowledge. To get started, begin with an example SPARQL query as described in the following steps:

1. Go to the SPARQL interface at [https://query.wikidata.org/](https://query.wikidata.org/).
2. Click on _Examples_ and scroll down to "Humans born in New York City." Select this to prefill your SPARQL query (Figure 19).

![](RackMultipart20220809-1-5enz3r_html_be6325e3e65b1391.png)

Figure 19. Screenshot from Wikidata Query Service ([https://query.wikidata.org/](https://query.wikidata.org/), retrieved 2022-05-11) showing the SPARQL query interface with the "Humans born in New York City" example.

1. Change the property from "[place of birth (P19)](https://www.wikidata.org/wiki/Property:P19)" to "[occupation (P106)](https://www.wikidata.org/wiki/Property:P106)." Change the item from "[New York City (Q60)](https://www.wikidata.org/wiki/Q60)" to "[paleontologist (Q1662561)](https://www.wikidata.org/wiki/Q1662561)" (Figure 20).

![](RackMultipart20220809-1-5enz3r_html_f49ebad2614f9d31.png)

Figure 20. Screenshot from Wikidata Query Service ([https://query.wikidata.org/](https://query.wikidata.org/), retrieved 2022-05-11) showing the SPARQL query interface with changes in the property and item fields to have the query search for Wikidata items with an occupation of paleontologist.

1. Click the blue square with the triangle on the left side to execute the query. This will generate a list of Wikidata items that have an "[occupation (P106)](https://www.wikidata.org/wiki/Property:P106)" that matches "[paleontologist (Q1662561)](https://www.wikidata.org/wiki/Q1662561)."
2. Search within these results for a particular item. For example, search for the text value "Schuchert." (Figure 21).

![](RackMultipart20220809-1-5enz3r_html_dfdc4efb8df8130c.png)

Figure 21. Screenshot from Wikidata Query Service ([https://query.wikidata.org/](https://query.wikidata.org/), retrieved 2022-05-11) illustrating where to search within the results of a query.

See these example queries (note that you need to click the blue square with the triangle on the left side to execute each query):

- [Here](https://query.wikidata.org/#%23%20Species%20of%20Isotelus%20%28trilobite%29%20with%20image%20if%20available%0A%0ASELECT%20%3Fitem%20%3Ftaxonname%20%3Fimage%20WHERE%20%7B%0A%20%20%3Fitem%20wdt%3AP31%20wd%3AQ16521%3B%0A%20%20%20%20wdt%3AP105%20wd%3AQ7432%3B%0A%20%20%20%20%28wdt%3AP171%2A%29%20wd%3AQ44087%3B%0A%20%20%20%20wdt%3AP225%20%3Ftaxonname.%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP18%20%3Fimage%20%7D%0A%7D) is a simple query for species of _Isotelus_ (a trilobite), where if the item has an image it is displayed in the query results.

- [Here](https://query.wikidata.org/#%23female%20paleontologists%20and%20fossil%20collectors%20born%3C1900%2C%20sorted%20by%20number%20of%20sitelinks%2C%20with%20some%20related%20info%0A%23%0ASELECT%20%3Fitem%20%3FitemLabel%20%28SAMPLE%28%3Foccname%29%20AS%20%3Foccname%29%20%3Fsitelinks%20%3FWDstatements%20%3Farticle%20%28SAMPLE%28%3Fbirth%29%20AS%20%3Fbirth%29%20%28SAMPLE%28%3Fdeath%29%20AS%20%3Fdeath%29%20%28SAMPLE%28%3Fbionomia%29%20AS%20%3Fbionomia%29%20WHERE%20%7B%0A%20%20%23%3Focc%20wdt%3AP279%7Cwdt%3AP279%2Fwdt%3AP279%2A%20wd%3AQ2374149.%0A%20%20VALUES%20%3Focc%20%7B%20wd%3AQ1662561%20wd%3AQ18624170%20%7D%0A%20%20%3Fitem%20wdt%3AP106%20%3Focc%20.%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP108%20%3Femp%20.%20%7D%0A%20%20%3Fitem%20wdt%3AP21%20wd%3AQ6581072%3B%0A%20%20%20%20wikibase%3Astatements%20%3FWDstatements%3B%0A%20%20%20%20wikibase%3Asitelinks%20%3Fsitelinks.%0A%20%20OPTIONAL%20%7B%0A%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%3B%0A%20%20%20%20%20%20schema%3AinLanguage%20%22en%22%3B%0A%20%20%20%20%20%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E.%0A%20%20%7D%0A%20%20%3Focc%20rdfs%3Alabel%20%3Foccname%20.%0A%20%20OPTIONAL%20%7B%3Fitem%20wdt%3AP569%20%3Fbirth%20.%7D%0A%20%20OPTIONAL%20%7B%3Fitem%20wdt%3AP570%20%3Fdeath%20.%7D%0A%20%20OPTIONAL%20%7B%3Fitem%20wdt%3AP6944%20%3Fbionomia%20.%7D%0A%20%20FILTER%28LANG%28%3Foccname%29%20%3D%20%22en%22%29.%0A%20%20FILTER%28%28%3Fbirth%3C%221900-01-01T00%3A00%3A00Z%22%5E%5Exsd%3AdateTime%29%7C%7C%28%3Fdeath%3C%221920-01-01T00%3A00%3A00Z%22%5E%5Exsd%3AdateTime%29%29.%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%0A%20%20%20%20bd%3AserviceParam%20wikibase%3Alanguage%20%22en%22%20.%0A%20%20%7D%0A%7D%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3Fsitelinks%20%3FWDstatements%20%3Farticle%0AORDER%20BY%20DESC%20%28%3Fsitelinks%29) is a more advanced query for female paleontologists and fossil collectors born before 1900, sorted by number of Wiki sitelinks, with some related information including Bionomia identifiers.

## Using Wikidata outside of Wikidata

As a shared knowledge platform, Wikidata is a powerful tool for linking information coming from disparate sources and enabling community curated data that can improve data quality elsewhere. Wikidata identifiers ([also called "QIDs"](https://www.wikidata.org/wiki/Q43649390)) provide a mechanism for connecting entities. While collections continue to enhance their local records and disambiguate data points like names of collectors or identifiers, inclusion of a Wikidata identifier in local collection information systems both provides an element of certainty in that record and enables future integration with the Linked Open Data ecosphere.

![](RackMultipart20220809-1-5enz3r_html_53155942663a9afe.jpg)

Figure 22. Screenshot of the Parties module in EMu at the Yale Peabody Museum showing the Wikidata identifier stored in the record.

Wikidata identifiers also can serve as appropriate values to use in the Darwin Core standard terms [recordedByID](http://rs.tdwg.org/dwc/terms/recordedByID) and [identifiedByID](http://rs.tdwg.org/dwc/terms/identifiedByID). When implementing the use of Wikidata outside of Wikidata, use the concept URI rather than the item page as the identifier value (e.g., [http://www.wikidata.org/entity/Q1039034](http://www.wikidata.org/entity/Q1039034) vs. [https://www.wikidata.org/wiki/Q1039034](https://www.wikidata.org/wiki/Q1039034)).

## Exporting from Wikidata in bulk

Several primary mechanisms are available for external, read-only access to information stored on Wikidata. These are briefly explained below.

### Export with Wikidata Query Service

The Wikidata Query Service (WDQS) is a SPARQL server instance for access to Wikidata. SPARQL is a language used to query data stored in RDF format. Queries are written in a specific format that adheres to the RDF specification, in contrast to the popular SQL query language.

Access Wikidata Query Service: [https://wikitech.wikimedia.org/wiki/Wikidata\_Query\_Service](https://wikitech.wikimedia.org/wiki/Wikidata_Query_Service)

See Wikidata Query Service documentation: [https://www.mediawiki.org/wiki/Wikidata\_Query\_Service/User\_Manual](https://www.mediawiki.org/wiki/Wikidata_Query_Service/User_Manual)

See more resources for learning how to use the Wikidata Query Service:

- A comparison between SQL and SPARQL, [https://cambridgesemantics.com/blog/semantic-university/learn-sparql/sparql-vs-sql/](https://cambridgesemantics.com/blog/semantic-university/learn-sparql/sparql-vs-sql/)
- Wikidata Data Model, [https://www.mediawiki.org/wiki/Wikibase/DataModel/Primer](https://www.mediawiki.org/wiki/Wikibase/DataModel/Primer)
- Wikidata Data Access, [https://www.wikidata.org/wiki/Wikidata:Data\_access](https://www.wikidata.org/wiki/Wikidata:Data_access)

### Export with MediaWiki Action API

Wikidata is based on the MediaWiki platform. As a result, many of the tools available for accessing MediaWiki are also available for Wikidata, including the official stable API called the MediaWiki Action API.

See API documentation: [https://www.wikidata.org/w/api.php](https://www.wikidata.org/w/api.php)

### Export with REST API

A third party REST API built on top of Wikidata SPARQL endpoints allows read-only access to Wikidata. This API is not officially supported by the Wikimedia Foundation, although the underlying SPARQL endpoints are provided by the foundation.

See API documentation: [https://opencitations.net/wikidata/api/v1](https://opencitations.net/wikidata/api/v1)

### Export with JSON data dump

Wikidata releases a regular snapshot, or "data dump," of the entire site as a single JSON file, which is available as \*.gz or \*.bz2 compressed formats. The uncompressed JSON files are large (\>100 GB) and therefore cannot be opened in a text editor.

Access JSON data dump files, arranged by timestamp: [https://dumps.wikimedia.org/wikidatawiki/entities/](https://dumps.wikimedia.org/wikidatawiki/entities/)

See documentation about the canonical JSON format used to represent Wikidata entities: [https://doc.wikimedia.org/Wikibase/master/php/md\_docs\_topics\_json.html](https://doc.wikimedia.org/Wikibase/master/php/md_docs_topics_json.html)

See documentation about Wikidata data dumps: [https://www.wikidata.org/wiki/Wikidata:Database\_download](https://www.wikidata.org/wiki/Wikidata:Database_download)

See these programmatic library resources for working with uncompressed JSON files:

- Go Programming Language, [https://gitlab.com/tozd/go/mediawiki](https://gitlab.com/tozd/go/mediawiki)
- PHP, [https://github.com/JeroenDeDauw/JsonDumpReader](https://github.com/JeroenDeDauw/JsonDumpReader)

### Export with RDF data dump

Wikidata releases a regular snapshot, or "data dump," of the entire site as a single RDF file using the Turtle and N-Triple formats. In addition, Wikidata entries labeled as "truthy" statements are available; truthy statements do not contain metadata such as qualifiers and references.

Access RDF data dump files: [https://dumps.wikimedia.org/wikidatawiki/entities/](https://dumps.wikimedia.org/wikidatawiki/entities/)

See documentation about the RDF format used to represent Wikidata entities: [https://www.mediawiki.org/wiki/Wikibase/Indexing/RDF\_Dump\_Format](https://www.mediawiki.org/wiki/Wikibase/Indexing/RDF_Dump_Format)

See documentation about Wikidata data dumps: [https://www.wikidata.org/wiki/Wikidata:Database\_download](https://www.wikidata.org/wiki/Wikidata:Database_download)

See these additional resources related to RDF:

- Turtle format, [https://www.w3.org/TR/turtle/](https://www.w3.org/TR/turtle/)
- N-Triple format, [https://www.w3.org/TR/n-triples/](https://www.w3.org/TR/n-triples/) and [https://en.wikipedia.org/wiki/N-Triples](https://en.wikipedia.org/wiki/N-Triples)
- Difference between RDF formats, [https://medium.com/wallscope/understanding-linked-data-formats-rdf-xml-vs-turtle-vs-n-triples-eb931dbe9827](https://medium.com/wallscope/understanding-linked-data-formats-rdf-xml-vs-turtle-vs-n-triples-eb931dbe9827)

## Wikidata Toolkit

The Wikidata Toolkit is an open source Java library and client that allows developers to build tools with direct access to Wikidata. Currently, the toolkit can be implemented either as a traditional Java library for Java-based applications, or as a standalone command-line interface client.

See documentation for the Wikidata Toolkit: [https://www.mediawiki.org/wiki/Wikidata\_Toolkit](https://www.mediawiki.org/wiki/Wikidata_Toolkit)

See also the Wikidata Toolkit GitHub repository: [https://github.com/Wikidata/Wikidata-Toolkit](https://github.com/Wikidata/Wikidata-Toolkit)

## Resources

## Resources for discovering biographical information

Most resources below can be searched to find biographical information about people in general. Several resources are particularly useful for finding data about people associated with paleontology collections. These data can be used to create more robust Wikidata items about people.

**Ancestry** ([https://www.ancestry.com](https://www.ancestry.com/))

Genealogical information. Particularly helpful for birth and death dates. Requires a paid account, but can often be accessed for free via your public library.

**BEMON** ([https://www.bemon.loven.gu.se](https://www.bemon.loven.gu.se/))

Biographical Etymology of Marine Organism Names (BEMON). Source for biographies of taxonomists working with marine organisms.

**Biodiversity Heritage Library** ([https://www.biodiversitylibrary.org](https://www.biodiversitylibrary.org/))

Access to digitized historical literature related to biodiversity. Source for biographies and research articles published in historical academic journals.

**Bionomia** ([https://bionomia.net](https://bionomia.net/))

Platform for linking biodiversity specimens to the people who collected and identified them. Pulls data for known people from Wikidata and ORCID. Source for exploring specimen data with people as the entry point.

**Cushman Foundation for Foraminiferal Research** ([https://cushmanfoundation.org/PersonifyEbusiness/Awards-Grants/General-Awards](https://cushmanfoundation.org/PersonifyEbusiness/Awards-Grants/General-Awards))

Source for recipients of various research awards related to foraminifera. See links related to each specific award.

**FamilySearch** ([https://www.familysearch.org/en](https://www.familysearch.org/en/))

Genealogical information. Particularly helpful for birth and death dates. Requires a free account. Source for digitized historical records and images.

**Find a Grave** ([https://www.findagrave.com](https://www.findagrave.com/))

Genealogical information. Particularly helpful for birth and death dates. Often includes images of headstones.

**FreeBMD** ([https://www.freebmd.org.uk](https://www.freebmd.org.uk/))

Source for information from the Civil Registration index of births, marriages and deaths for England and Wales.

**GSA Memorials** ([https://www.geosociety.org/gsa/pubs/memorials.aspx](https://www.geosociety.org/gsa/pubs/memorials.aspx))

Tributes written by associates, friends, or relatives to deceased members of the Geological Society of America. Relevant only to a limited number of individuals, but an excellent source with detailed information.

**Internet Archive** ([https://archive.org](https://archive.org/))

Non-profit searchable library of millions of free digitized books, movies, software, music, websites, and more.

**JSTOR** ([https://www.jstor.org/](https://www.jstor.org/))

Source for digitized journal articles, books, images, and primary sources.

**National Academy Memoirs** ([http://www.nasonline.org/publications/biographical-memoirs](http://www.nasonline.org/publications/biographical-memoirs/))

Source for life histories and selected bibliographies of deceased National Academy of Sciences members. Relevant only to a limited number of individuals, but an excellent source with detailed information.

**ORCID** ([https://orcid.org](https://orcid.org/))

Platform for assigning persistent digital identifiers to living people. Source for detailed work history information, including institutional affiliations and publications.

**PapersPast** ([https://paperspast.natlib.govt.nz/newspapers](https://paperspast.natlib.govt.nz/newspapers))

Source for full-text newspaper articles published in New Zealand, some of which may represent articles still protected by copyright in the United States.

**Zoobank** ([https://zoobank.org](http://zoobank.org/))

Official Registry of Zoological Nomenclature. Source for evidence of a person contributing to nomenclature, e.g., via publishing an original description of a new species.

## Resources for using Wikidata

Many excellent resources exist for learning how to use Wikidata, and for using Wikidata more efficiently. Those included below provide a starting point.

**Author Disambiguator** ([https://author-disambiguator.toolforge.org](https://author-disambiguator.toolforge.org/))

This tool is a visual interface for editing Wikidata items representing the authors of works also recorded in Wikidata. In particular, it aims to assist users in converting author names from strings to items. The Author Disambiguator is integrated with Scholia (see below).

**Cradle** ([https://cradle.toolforge.org](https://cradle.toolforge.org/))

This tool allows users to create new Wikidata items from a form, saving the time typically required to remember and enter all of the relevant statement properties. For example, a user may wish to use Cradle as a template for a new Wikidata item representing a [scientific thesis](https://www.wikidata.org/wiki/Wikidata:Cradle#Thesis).

**Library Carpentry Wikidata** ([https://librarycarpentry.org/lc-wikidata](https://librarycarpentry.org/lc-wikidata))

"This Library Carpentry lesson introduces librarians to Wikidata. At the conclusion of the lesson you will: know what the Wikidata interface looks like; know how Wikidata is linked to other Wiki projects; know the underlying concepts of Wikidata; create and develop Wikidata items yourself; add references to Wikidata; create a search query in Wikidata using the query language SPARQL; understand how to perform a mass import into Wikidata."

**Training aids and resources curated by Aotearoa New Zealand Online** ([https://en.wikipedia.org/wiki/Wikipedia:Meetup/Aotearoa\_New\_Zealand\_Online](https://en.wikipedia.org/wiki/Wikipedia:Meetup/Aotearoa_New_Zealand_Online))

Scroll down to the "Training aids and resources" section for links to resources that are thoughtfully curated, and actively updated, by this community.

**YouTube videos produced by the Wikimedian in Residence at the University of Edinburgh** ([https://www.youtube.com/channel/UCSDRSVKM4ceUSPI-7-BFeoQ/videos](https://www.youtube.com/channel/UCSDRSVKM4ceUSPI-7-BFeoQ/videos))

Good visual tutorials for basic Wikidata editing. Recommended videos include [How to add a new item to Wikidata](https://www.youtube.com/watch?v=3CuUgJK4L78) and [Adding manual edits to Wikidata: how to add statements with verifiable data and how to create items](https://www.youtube.com/watch?v=ibUzIHztZiQ).

## Resources for exploring Wikidata

Exploring the data in Wikidata is an exciting way to both answer questions and envision new possibilities.

**Mix'n'match** ([https://mix-n-match.toolforge.org](https://mix-n-match.toolforge.org/))

This tool allows users to explore data in and external to Wikidata through a visual, gamified interface.

**Scholia** ([https://scholia.toolforge.org/](https://scholia.toolforge.org/))

"Scholia is a service that creates visual scholarly profiles for topics, people, organizations, species, chemicals, etc. using bibliographic and other information in Wikidata."

## Resources for getting involved in the Wikimedia community

There are numerous active subsets of the community using Wikidata, and participating in one or more of them can be a good way to solidify skills and to make connections with other people.

**LD4 Wikidata Affinity Group** ([https://www.wikidata.org/wiki/Wikidata:WikiProject\_LD4\_Wikidata\_Affinity\_Group](https://www.wikidata.org/wiki/Wikidata:WikiProject_LD4_Wikidata_Affinity_Group))

LD4 collaborates to advance library and archival practices with a focus on linked open data. The LD4 Wikidata Affinity Group hosts "discussion of Wikidata related topics with the goal of understanding how the library can contribute to and leverage Wikidata as a platform for publishing, linking, and enriching library linked data." They have regular online meetings and an active Slack channel.

**WikiConference North America** ([https://wikiconference.org](https://wikiconference.org/))

"WikiConference North America is the annual conference of Wikimedia enthusiasts and volunteers from throughout North America, including Canada, the United States, Mexico, and the Caribbean. Join Wikipedia, -media, -data, and -cite enthusiasts for a long weekend of collaboration and discovery!" See annual meeting information on the website linked above.

**WikiCon** ([https://meta.wikimedia.org/wiki/WikiCon](https://meta.wikimedia.org/wiki/WikiCon))

This landing page provides direction to Wikimedia conferences happening globally.

## Conclusion

Work to enhance and create items in Wikidata is ongoing. By contributing, you are engaging in a community process to improve and build open knowledge about our collections and the people associated with them. Edits in Wikidata directly impact the specimen information mobilized by collections through local implementation of Wikidata identifiers. Within Wikidata, the web of information being built by users like you can be seen by exploring how a Wikidata item is linked throughout the platform. For an example, see this [list of other items that link to the item for](https://www.wikidata.org/w/index.php?title=Special%3AWhatLinksHere&target=Q19865330&namespace=)[Wilmatte Porter Cockerell](https://www.wikidata.org/w/index.php?title=Special%3AWhatLinksHere&target=Q19865330&namespace=).

If you would like to participate in the ongoing work of the paleo collections community and the _Using Wikidata to Capture and Share Information about People in Paleontology_ workshop, please visit our GitHub page and consider adding to our growing [list of People in Paleontology](https://docs.google.com/spreadsheets/d/1v9sLu-8GuTN8kOEWSHhZkPWRiZ2-a-s4MeqSEmqos1A/edit?usp=sharing).
