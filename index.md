---
title: Essential Components of Web Accessibility
permalink: /fundamentals/components/
github:
  repository: w3c/wai-components
layout: default
footer: >
  <p>
    <strong>Permission to use:</strong> 
    You may use the images on this page for accessibility education and outreach if you: 
    1. Include the URI <strong><span class="changed">w3.org/WAI/intro/components.php</span> <em>prominently</em></strong> near the image, and 
    2. Include the artist credit, editor, and copyright reference in any published or posted material:<br>
    <cite>Image by Michael Duffy, from: Essential Components of Web  Accessibility. S.L. Henry, ed. Copyright W3C <sup>®</sup> (MIT, ERCIM, Keio, Beihang). w3.org/WAI/intro/components.php</cite><br>
    For more information, see <a href="https://www.w3.org/WAI/about/usingWAImaterial.html">Using WAI Materials</a>.
  </p>
  <p><strong>Date: </strong>Updated 27 February 2018. <!--[<a href="https://www.w3.org/WAI/EO/changelogs/cl-components">changelog</a>]--></p>
  <p><strong>Editor:</strong> <a href="http://www.w3.org/People/Shawn">Shawn Lawton Henry</a>. Graphic artist: Michael Duffy.</p>
  <p>Developed with input from the Education and Outreach Working Group (<a href="http://www.w3.org/WAI/EO/">EOWG</a>).</p>

---

{::nomarkdown}
{% include box.html type="start" h="2" title="Summary" class="full" %}
{:/}

This page shows how web accessibility depends on several components working together, and how improvements in specific components could substantially improve web accessibility.

It provides the foundation for understanding the different accessibility standards developed by the <abbr title="World Wide Web Consortium">W3C</abbr> Web Accessibility Initiative (WAI).

{::nomarkdown}
{% include box.html type="end" %}
{:/}

{::nomarkdown}
{% include_cached toc.html type="start" title="Page Contents" class="simple" %}
{:/}

{::options toc_levels="2" /}

-   This text will be replaced by the TOC.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}


## Introduction {#intro}
{:.no_toc}

It is essential that several different components of web development and
interaction work together in order for the web to be accessible to
people with disabilities. These components include:

-   **content** - the information in a web page or web application,
    including:
    -   natural information such as text, images, and sounds
    -   code or markup that defines structure, presentation, etc.
-   **web browsers, media players**, and other "user agents"
-   **assistive technology**, in some cases - screen readers,
    alternative keyboards, switches, scanning software, etc.
-   **users**' knowledge, experiences, and in some cases, adaptive
    strategies using the web
-   **developers** - designers, coders, authors, etc., including
    developers with disabilities and users who contribute content
-   **authoring tools** - software that creates websites
-   **evaluation tools** - web accessibility evaluation tools, HTML
    validators, CSS validators, etc.

## How the Components Relate {#relate}

{% assign example_url = "/fundamentals/components/examples/#relate" | relative_url %}
![illustration showing how components relate, detailed description at {{ example_url }}]({{ "/content-images/wai-components/relate.png" | relative_url }}){:longdesc="{{example_url}}"}

Web **developers** usually use **authoring tools** and evaluation tools
to create web **content**.

**People** ("**users**") use web **browsers, media players, assistive
technologies,** or other "**user agents**" to get and interact with the
**content**.

## Interdependencies Between Components {#depend}

There are significant interdependencies between the components; that is,
the components must work together in order for the web to be accessible.
For example, for alternative text on images:

-   **technical specifications** address alternative text (for example,
    HTML defines the alternative text attribute (alt) of the image
    element (img))
-   **WAI guidelines** ([WCAG, ATAG, UAAG described
    below](#guidelines)) - define how to implement alternative text for
    accessibility in the different components
-   **developers** provide the appropriate alternative text wording
-   **authoring tools** enable, facilitate, and promote providing
    alternative text in a web page
-   **evaluation tools** are used to help check that alternative text
    exists
-   **user agents** provide human and machine interface to the
    alternative text
-   **assistive technologies** provide human interface to the
    alternative text in various modalities
-   **users** know how to get the alternative text from their user agent
    and/or assistive technology as needed

### The Implementation Cycle

When accessibility features are effectively implemented in one
component, the other components are more likely to implement them.

{% assign example_url = "/fundamentals/components/examples/#cycle" | relative_url %}
![illustration of implementation cycle, detailed description at {{ example_url }}]({{ "/content-images/wai-components/cycle.png" | relative_url }}){:longdesc="{{example_url}}"}

-   When **web browsers, media players, assistive technologies, and
    other user agents** support an accessibility feature, users are more
    likely to demand it and developers are more likely to implement it
    in their **content**.
-   When developers want to implement an accessibility feature in their
    **content**, they are more likely to demand that their **authoring
    tool** make it easy to implement.
-   When **authoring tools** make a feature easy to implement,
    developers are more likely to implement it in their **content**.
-   When an accessibility feature is implemented in **most content**,
    developers and users are more likely to demand that **user agents**
    support it.

### When One Component is Weak

If an accessibility feature is not implemented in one component, there
is little motivation for the other components to implement it when it
does not result in an accessible user experience. For example,
developers are unlikely to implement an accessibility feature that
authoring tools do not support and that most browsers or assistive
technologies do not implement consistently.

{% assign example_url = "/fundamentals/components/examples/#bridge" | relative_url %}
![illustration of what happens when one component is weak, detailed
description at {{ example_url }}]({{ "/content-images/wai-components/bridge.png" | relative_url }}){:longdesc="{{example_url}}"}

If one component has poor accessibility support, sometimes other
components can compensate through "work-arounds" that require much more
effort and are not good for accessibility overall. For example,

-   developers can do more work to compensate for some lack of
    accessibility support in authoring tools; for example, coding markup
    directly instead of through a tool
-   users can do more work to compensate for some lack of accessibility
    support in browsers, media players, and assistive technology and
    lack of accessibility of content; for example, using different
    browsers or assistive technologies to overcome different
    accessibility issues

However, in most cases the works-arounds are not implemented and the
result is still poor accessibility. Additionally, sometimes poor
accessibility support in one component cannot be reasonably overcome by
other components and the result is inaccessibility, making it impossible
for some people with disabilities to use a particular website, page, or
feature.

## Guidelines and Other Standards {#guidelines}

The World Wide Web Consortium ([W3C](https://www.w3.org/)) Web Accessibility Initiative ([WAI](https://www.w3.org/WAI/)) develops **web accessibility standards** for the different components:

-   [Authoring Tool Accessibility Guidelines (**ATAG**)](atag.php)
    addresses authoring tools
-   [Web Content Accessibility Guidelines (**WCAG**)](wcag.php)
    addresses web content, and is used by developers, authoring tools,
    and accessibility evaluation tools
-   [User Agent Accessibility Guidelines (**UAAG**)](uaag.php) addresses
    web browsers and media players, including some aspects of assistive
    technologies

<p>These accessibility guidelines are based on the fundamental technical specifications of the web, and are developed in coordination with all <a href="https://www.w3.org/TR/">W3C technical specifications</a> (HTML, XML, CSS, SVG, SMIL, etc.). W3C also develops technical specifications that directly address accessibility, including:</p>
<ul>
  <li><a href="https://w3c.github.io/wai-website/standards/aria/">ARIA, the Accessible Rich Internet Applications</a> Suite, which defines a way to make web applications more accessible to people with disabilities. It especially helps with dynamic content and advanced user interface controls developed with Ajax, HTML, JavaScript, and related technologies.</li>
</ul>

{% assign example_url = "/fundamentals/components/examples/#guide" | relative_url %}
![illustration showing the guidelines for the different components, detailed description at {{ example_url }}]({{ "/content-images/wai-components/specs.png" | relative_url }}){:longdesc="{{example_url}}"}

For more information, see [W3C Accessibility Standards Overview](https://w3c.github.io/wai-std-gl-overview/standards-guidelines/)
