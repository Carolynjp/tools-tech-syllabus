.. _DITA Introduction:

DITA Introduction
#############################


Goals
*********

* Understand the philosophy and goals of DITA.
* Understand the basic DITA topic types.

Introduction
*************

.. include:: slideshare/dita_intro.txt

Readings
*********

* |DITA - Wikipedia|

* |DITA Tutorial|

* |DITA FAQs|

* |DITA Concepts|

Videos
*******

.. youtube:: ngHIIWbEp_Q?list=PL6798EBA382414741

.. include:: snippets/video_series.txt


Assignment
************

|Assignment|

#. In the repository you made in :ref:`XML`, create a new branch.

#. Modify the XML file you created to be a valid DITA topic.

   For this exercise, make the topic a **concept**.

   For example, you could modify the document from the preview lesson:

   .. code-block:: XML
     :linenos:

      <page>
        <author>Your name</author>
        <title>The Title</title>
        <abstract>Two sentence abstract.</abstract>
        <body>
        <paragraph>First paragraph</paragraph>
        <paragraph>Second paragraph</pargraph>
      </body>
      </page>

   Into a DITA concept.

   .. code-block:: XML
     :linenos:

      <!DOCTYPE concept
      PUBLIC '-//OASIS//DTD DITA Concept//EN'
      'dtd1.2/technicalContent/dtd/concept.dtd'>
      <concept id="sample_concept" xml:lang="en-US">
        <author>Your name</author>
        <title>My Abstract</title>
        <shortdesc>My Abstract</shortdesc>
        <conbody>
          <p>First paragraph</p>
          <p>Second paragraph</p>
        </conbody>
       </concept>  

   Use valid elements for a concept.

#. Validate the file against the DTD for the topic type.

   .. note:: You must set the ``DOCTYPE`` declaration to the path and name of the DTD. Take a look at the sample files in the |Get Started with DITA repository|.  Copy the ``dtd1.2`` folder from there into your branch, and validate your file against the concpet, task, or 

.. include:: snippets/save_github.txt

.. include:: includes.txt
