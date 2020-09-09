# MarketGardenCropPlanner

What is this tool and what can it do?

This is a business and operations planning tool designed for consumer-supported agriculture (CSA) farms. The basic business model is that customers buy farm products on a subscription basis, with deliveries being made on a weekly or bi-weekly basis. 

This tool attempts to answer the following questions:
1.	What can I plant in my area?
2.	When should I plant these crops?
3.	When will they be ready?
4.	How should I price my CSA shares?
5.	What is the financial outlook of my farm?

To answer the above questions, this tool performs the following functions:
1.	Organize reference data on the Planting Constraints, DS (Direct Seeding) Crop Ref, and TP (Transplant) Crop Ref sheets.
  a.	This reference data is going to vary with the local climate conditions. I would recommend reviewing and updating this data if any of the later calculations don’t pass the sniff test.

2.	Business planning: On the Annual Input sheet, users can adjust the input parameters (highlighted cells) to model the finances of their farm. 
  a.	The Planning Period Start and Planning Period End values are by default set to 1 year. If you want to plan out multiple seasons at a time, you may extend this to 2 or more years.

3.	CSA Share Modelling: After validating the reference data and clicking the Recalculate Availability button on the Intro sheet, the workbook will calculate when your crops will be available (represented by green cells on the Weekly CSA Share Content sheet).
  a.	By default, the workbook will order one unit of each available crop. That is, if you’re tracking tomato yield by the pound and your tomatoes are available for 10 weeks in the season, then each CSA share will be allocated 10 pounds of tomatoes.
    i.	If the ‘one-of-each’ allocation isn’t practical, you may change then ordered quantity by changing the numbers on the Weekly CSA Share Content sheet. Fractional values are accepted.
  b.	As you add and subtract items from your weekly CSA shares, you’ll notice the two summary rows at the bottom of the sheet are keeping track of how much each share is worth. This information is used to calculate the average Weekly CSA Share price in cell B1 of the Annual plan sheet.

4.	Farm Operations Planning: Once you have customized your weekly CSA shares, you can click the Create Farm Plan button on the Intro sheet to generate a consolidated operations calendar along with seed orders, greenhouse and crop schedules, and weekly harvest targets.
  a.	Calendar – This sheet offers a consolidated weekly schedule of Field Prep, Greenhouse, and Field Planting work.
  b.	Weekly CSA Harvest Target – This sheet simply multiplies the Weekly CSA Share Content table by the number of shares offered. 
  c.	Seed Sheet – This sheet calculates the amount of seed needed for each crop this season.
  d.	Greenhouse Schedule – This sheet calculates the number of trays each transplanted crop needs in the greenhouse and on what days they should be started.
  e.	Crop Sheet – This sheet calculates the planting frequency and quantity for each crop in order to meet the weekly harvest targets.
  f.	Field Ops – This sheet calculates the field prep dates for the various planting groups outlined in the Crop Sheet.
  g.	Field Planting Schedule – This sheet provides weekly summaries of the amount of planting needed to meet the weekly harvest targets. Mostly, it is used in the Crop Sheet calculations.


If you have any questions about how this tool functions or the code it uses, reach out to Gavin O’Leary on the Permies.com forums. 

If you want to learn more about market gardening, these two books inspired much of the design and layout of this tool:
1.	The Market Gardener – Jean-Martin Fortier
2.	Crop Planning for Vegetable Growers - Frederic Theriault & Daniel Brisebois

