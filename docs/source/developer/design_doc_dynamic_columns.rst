HLM-FATES Dynamic Columns Design
================================

Introduction
------------
.. Discuss the design origins, intent and goals.  What is the problem statement?  If there are any specification documents, link them in Appendix.

The goal of this software design update is to allow fates to operate on multiple soil columns on a given gridcell.

Design Considerations
---------------------
.. Describe the issues that need to be addressed before creating a design solution.

Assumptions and Dependencies
^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. Describe any assumptions that may be wrong or any dependencies on other things

General Constraints
^^^^^^^^^^^^^^^^^^^
.. Describe any constraints that could have an impact on the design of the software.

Solutions
---------
.. Section should include alternative implementations/solutions.  Is it feasible? How much effort does it need for each approach? Pros/cons of each approach.  Document alternatives, why you made the decision and how it will affect the team and project.

Design and Architecture
-----------------------
..  Provide a general overview of the software layout

System diagram or flowchart
^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. Interaction diagram of various inputs, outputs, sub systems and dependencies.

Algorithm or Pseudo code for main components
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
.. Describe your logic in this section.  See https://pypi.org/project/sphinxcontrib-pseudocode/ for links to documentation.

Rollout Plan
------------
.. Define the roll-out phases and tests you plan to do

Initial Steps:

- 0, 1 weighted column
- split fractional columns and confirm sums across columns

NGEE-T land use columns
- primary land columns and everything else (gross flux)
- primarylands columns, secondarylands columns (net transitions)

NGEE-A time-since-fire
- two bins: above and below some age value
- multiple bins

Soil temp, moisture, nutrients are the soil states values

active layer = depth things thaw in summer time

v0: Columns are associated with a specific time-since-fire age bin.
v1: Columns associated with a specific land use type as well

Future Update Plan
------------------
.. Sketch out future updates if known

Implementation Notes and Lessons Learned
----------------------------------------
.. Optional section summarizing lessons learned after the design has been successfully implemented

Appendix
--------
.. References, links to additional documentation
