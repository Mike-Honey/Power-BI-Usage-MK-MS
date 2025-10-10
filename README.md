# Power-BI-Usage-MK-MS
**Power BI usage analysis via Measure Killer, by Manga Solutions**

[Measure Killer](https://www.brunner.bi/measurekiller) is a tool developed by Burnner BI, as a solution for exploring the used and unused objects within Power BI Reports.

To help solve problems for the clients of my [Manga Solutions](www.mangasolutions.com) consulting practice, I have created a Power BI report to integrate and analyse the usage data that can be exported from Measure Killer. 

## Usage page 

[Link to interactive DataViz](https://app.powerbi.com/view?r=eyJrIjoiMDk2YjA4MjgtYjkzNC00NDZkLTgwODItOGZiMzVkMWQ2NzMxIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D)

[![Click to view and interact with the report](https://github.com/Mike-Honey/Power-BI-Usage-MK-MS/blob/main/Power-BI-Usage-MK-MS-Usage-Page.png?raw=true)](https://app.powerbi.com/view?r=eyJrIjoiMDk2YjA4MjgtYjkzNC00NDZkLTgwODItOGZiMzVkMWQ2NzMxIiwidCI6ImRjMWYwNGY1LWMxZTUtNDQyOS1hODEyLTU3OTNiZTQ1YmY5ZCIsImMiOjEwfQ%3D%3D)

The intended use of the **Summary** page is to quickly scan the connections between pages, visuals, tables, fields and measures, in any direction. Selecting any entry of any type will cross-filter all the other objects.  For example selecting a Page object will cross filter to show all the visuals on that page, and the tables, fields and measures that they reference. By contrast, selecting a Field  object will cross-filter to show the pages and visuals where it is used, and it's home table.

The format is intended for "business analyst" types and other non-technical users. As the solution is a Power BI report, it can be published to the Power BI web service or shared via SharePoint or OneDrive. This can provide near-instant and personalised access, without even needing to open the source PBIX/PBIP file, or install and run Measure Killer.  If you need to extend this solution further, the existing pages offer a transparent guide to the elements of the semantic model.

## How-To

Here's how to use this solution to analyse your own Power BI semantic models and reports :

1. Open the target Power BI semantic model file in [Power BI Desktop](https://www.microsoft.com/en-au/power-platform/products/power-bi/desktop)
2. Launch the [Measure Killer](https://www.brunner.bi/measurekiller) application, connect to your Power BI semantic model and reports, **Run** the process and then use the menu to Export in Excel format.
3. Optionally, close Power BI Desktop and Measure Killer
4. Open your copy of the PBIX file in this project, using Power BI Desktop. My naming standard is **[source PBIX/PBIP file name] - Power-BI-Usage-MK-MS.pbix**. For easy maintenance, I would save a copy of the PBIX file from this project for each source analysis I want to maintain.
5. In the Power BI window for the Power-BI-Usage-MK-MS file, navigate to **Transform data / Edit parameters**.
6. To get the value for the **ExcelExportFile** parameter, you can use Windows Explorer to navigate to the Exported Excel file, then right-click and choose **Copy as path**. After pasting that into Power BI, be sure to remove the leading and trailing quotes.
7. Hit **OK**, then **Apply Changes**.
8. Wait for the query to refresh, then save your Power-BI-Usage-MK-MS PBIX file.
9. Review your results in Power BI Desktop, or publish and share your Power-BI-Usage-MK-MS file using Power BI Web, SharePoint or OneDrive.

## Discussion

There are several other tools around now to help with similar tasks, and some of them have more features. This [article by SQLBI](https://www.sqlbi.com/articles/tools-in-power-bi/) gives a handy summary and describes each one. Measure Killer is a leading solution IMO. But those tools are mostly specific apps that must be installed and/or licensed, and they usually require some preparation work using Power BI Desktop before any results can be reviewed. Most are quite technical in style, not aimed at a "business analyst" / non-technical audience. None can be extended, customised or shared as easily as a PBIX file. So I believe there is still a niche for this solution.

The sample PBIX file provided was generated from my favourite demo file, the [Miradi template](https://github.com/Mike-Honey/miradi), which I maintain.  You can download that sample PBIX file from that project, or quickly view it online from that Project's page.

The design of the Summary page borrows heavily from my earlier project [Power-BI-Cleaner-MS](https://github.com/Mike-Honey/Power-BI-Cleaner-MS). This project takes advantage of Measure Killer's superior integration with Power BI (e.g. support for PBIP files and thin reports). I don't plan to reproduce the other pages from that project, as most of that functionality is already covered in the Measure Killer UI.  This project takes advantage of the extra data gathered by Measure Killer with some additional slicers, for Report and Category.

I welcome any ideas or contributions - you can start the discussion by raising an Issue.


## 🤝 Support

Contributions, issues, feature requests and sponsorship are all welcome!

Give a ⭐️ if you like this project!

